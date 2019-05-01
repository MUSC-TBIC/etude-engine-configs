Sample Runs
===========

Basic Run
---------

.. code:: bash

   export ETUDE_DIR=etude-engine
   export ETUDE_CONFIGS_DIR=etude-engine-configs
   
   export N2C2_DATA=/tmp/n2c2

   python ${ETUDE_DIR}/etude.py \
     --reference-input ${N2C2_DATA}/train_annotations \
      --reference-config ${ETUDE_CONFIGS_DIR}/n2c2/2018_n2c2_track-1.conf \
      --test-input ${N2C2_DATA}/train_annotations \
      --test-config ${ETUDE_CONFIGS_DIR}/n2c2/2018_n2c2_track-1.conf \
      --no-metrics \
      --print-custom "2018 n2c2 track 1" \
      --fuzzy-match-flag exact \
      --file-suffix ".xml" \
      --empty-value 0.0
   
   
   ******************************************* TRACK 1 ********************************************
                         ------------ met -------------    ------ not met -------    -- overall ---
                         Prec.   Rec.    Speci.  F(b=1)    Prec.   Rec.    F(b=1)    F(b=1)  AUC   
              Abdominal  1.0000  1.0000  1.0000  1.0000    1.0000  1.0000  1.0000    1.0000  1.0000
           Advanced-cad  1.0000  1.0000  0.0000  1.0000    0.0000  0.0000  0.0000    0.5000  0.5000
          Alcohol-abuse  0.0000  0.0000  1.0000  0.0000    1.0000  1.0000  1.0000    0.5000  0.5000
             Asp-for-mi  1.0000  1.0000  0.0000  1.0000    0.0000  0.0000  0.0000    0.5000  0.5000
             Creatinine  1.0000  1.0000  1.0000  1.0000    1.0000  1.0000  1.0000    1.0000  1.0000
          Dietsupp-2mos  1.0000  1.0000  1.0000  1.0000    1.0000  1.0000  1.0000    1.0000  1.0000
             Drug-abuse  0.0000  0.0000  1.0000  0.0000    1.0000  1.0000  1.0000    0.5000  0.5000
                English  1.0000  1.0000  0.0000  1.0000    0.0000  0.0000  0.0000    0.5000  0.5000
                  Hba1c  1.0000  1.0000  1.0000  1.0000    1.0000  1.0000  1.0000    1.0000  1.0000
               Keto-1yr  0.0000  0.0000  1.0000  0.0000    1.0000  1.0000  1.0000    0.5000  0.5000
         Major-diabetes  1.0000  1.0000  1.0000  1.0000    1.0000  1.0000  1.0000    1.0000  1.0000
        Makes-decisions  1.0000  1.0000  0.0000  1.0000    0.0000  0.0000  0.0000    0.5000  0.5000
                Mi-6mos  1.0000  1.0000  1.0000  1.0000    1.0000  1.0000  1.0000    1.0000  1.0000
                         ------------------------------    ----------------------    --------------
        Overall (micro)  1.0000  1.0000  1.0000  1.0000    1.0000  1.0000  1.0000    1.0000  1.0000
        Overall (macro)  0.7692  0.7692  0.6923  0.7692    0.6923  0.6923  0.6923    0.7308  0.7308
   
                                                       10 files found


# Model Definition and Evaluation

## Overview

Für die bakery predictions mithilfe von maschinellen Lernens wurden sechs neuronale Modell für jede der sechs Warengruppen implemtiert und mit den Features, welche für das Baseline Modell genutzt worden sind, trainiert.

Die Data Preparation wurde zweimal für die Daten [ohne](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Data preparation missing values.ipynb) und [mit](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Data preparation with data imputation.ipynb) Dataimputation über KNN durchgeführt. 

nput-Daten:
- ohne data impuation: [merged_data_new](/workspaces/DS_ML_Gr_1.5/2_BaselineModel/merged_data_new.csv) (siehe Baseline-Modell)
- mit KNN imputation: [Imputed_Data_KNN](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Imputed_Data_KNN.csv)

## Guidelines

- **Model Selection**
Sequential Modell mit batch normalization und dense layers (aus Keras)

- **Hyperparameter Tuning**
Die Hyperparameter wurden per Ausprobieren angepasst. 

    - [W1_Brot](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Neuronales_Netz_W1_Brot.ipynb)
        - Dense (10, activation='relu'),Dropout(.3), Dense(8, activation='relu'), Dense(6, activation='relu'), Dense(1)
        - Lernrate = 0.0018; Epochen =  24; Optimizer = ADAM
    - [W2_Broetchen](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Neuronales_Netz_W2_Broetchen.ipynb)
        - Dense (10, activation='relu'),Dropout(.3), Dense(8, activation='relu'), Dense(6, activation='relu'), Dense(1)
        - Lernrate = 0.0018; Epochen = 24; Optimizer = ADAM
    - [W3_Croissant](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Neuronales_Netz_W3_Croissants.ipynb)
        - Dense (125, activation=‘relu’), Dropout(.3), Dense(120, activation='relu'), Dense(120, activation='relu'), Dense(1)
        - Lernrate = 0.0018; Epochen = 100; Optimizer = ADAM
    - [W4_Konditorei](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Neuronales_Netz_W4_Konditorei.ipynb)
        - Dense (125, activation='relu'), Dropout(.3), Dense(110, activation='relu'), Dense(1)
        - Lernrate = 0.001; Epochen = 8; Optimizer = ADAM
    - [W5_Kuchen](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Neuronales_Netz_W5_Kuchen.ipynb)
        - Dense (225, activation=‘relu’), Dropout(.3), Dense(220, activation='relu'), Dense(220, activation='relu'), Dense(1)
        - Lernrate = 0.0018; Epochen = 100; Optimizer = ADAM
    - [W6_Saisonbrot](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/Neuronales_Netz_W6_Saisonbrot.ipynb)
        - Dense(17500, activation='relu'), Dropout(.5), Dense(4, activation='relu'), Dense(1)
        - Lernrate = 0.001; Epochen = 10000; Optimizer = ADAM

- **Implementation**
[K-Nearest Neighbors (KNN) imputation Methode](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/missing_value_imputation.ipynb)

- **Evaluation Metrics**
    - MAPE
    - Training and Validation loss function 

- **Data submission**
    - Für die data submission auf Kaggle wurden die Prediction Daten aus dem neuronalen Netztwerk in [BM-Data_export](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/BM-Data_export.ipynb) aufbereitet und die csv-Datei [sample_submission_NN.csv](/workspaces/DS_ML_Gr_1.5/3_Neuronal_Model/sample_submission_NN.csv) hochgeladen.

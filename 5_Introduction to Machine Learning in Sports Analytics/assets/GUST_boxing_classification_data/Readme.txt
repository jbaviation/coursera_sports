Boxing classication data - Griffith University Sports Technology (GUST)

Matthew Worsey - 17/02/2021

Inside this folder are 7 files:

The raw sensor data (prior to punch detection and feature extraction) is stored in:

Raw_sensor_training_data.xlsx and Raw_sensor_evaluation_data.xlsx 

Training data was the data used for model training (50 of each punch type) and evaluation data was the data used for model evaluation (82 punches in total - random order). 
Each excel file contains 3 sheets (left wrist data, right wrist data and upper back (T3) data), each sheet has 9 headers:

Acceleration in x axis, Acceleration in y axis and Acceleration in z axis
Gyro in x axis, Gyro in y axis, Gyro in z axis
Euler angles: Roll, pitch and yaw. 

Axes orientation of each sensor can be found in the published IoT paper.

------------------------------------------------------------------------------------------
The feature data (features extracted from detected punch window data) is stored in:
Training_features_T3_sensor.csv
Evaluation_features_T3_sensor.csv
Training_features_wrist_sensors.csv
Evaluation_features_wrist_sensors.csv

As we trained and evaluated models using two configuraitons (just the wrist sensors and just the T3 sensor [punches detected by wrist sensors]).
Training_features are the features used for model traning and evaluation_features are the features used for model evaluation.
The headers relate to the extracted features (e.g. mean, standard deviation, kurtosis of punch window Accel_x signal). 
These were the csv files used for training and evaluation in Python. 

----------------------------------------------------------------------------------------------------------------------------
Punch_orders_video_analysis.xlsx contains the punch-type order for both the training and evaluation data. 
The way my code extracted punch windows meant that left and right punches were stored together so please refer to this file when starting with the raw sensor data. 
However the punches in the feature data are labeled correctly. 
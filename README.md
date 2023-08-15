# Anomaly Detection Using LSTM-Autoencoder 
This repo contains files related to implementation of LSTM Autoencoder for anomaly detection using Tensorflow.

## Explanation
The goal was to detect a partial overlap between peg and a hole in a robotic assembly task. </br>
For that purpouse a real sensor data was collected from the robot and labeled. The sensor data consists of forces and moments.
As can be seen on the attached ilustration during partial overlap peaks are visible in the sensor measurements (in certain directions). 
The goal was to train the model to detect them!.

![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/bce3bbdb-8464-4b58-8465-2b4cad63a923)

## Model (LSTM-Autoencoder)
THe model used for this task is LSTM Autoencoder. 
LSTM are DNN that are able to model the short and long term dependanceies in data, therefore their use for time series data is justified. 

![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/a368b454-b62c-4cdc-978f-f4b7d294b79c)

![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/76da597b-aada-4bb3-a6eb-d394ba605e39)

![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/1b225097-e5f3-4d85-90a9-a2e2e42264f1)

![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/5c865cc1-ad2b-4de5-9bff-247bef43a14b)

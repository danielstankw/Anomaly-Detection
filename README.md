# Anomaly Detection Using LSTM-Autoencoder 
This repo contains files related to implementation of LSTM Autoencoder for anomaly detection using Tensorflow.

## File Content:
* sacsad
* dasad

## Task Explanation
The goal was to detect a partial overlap between peg and a hole in a robotic assembly task. </br>
For that purpouse a real sensor data was collected from the robot and labeled for accuracy measurement. The sensor data consisted of forces and moments as well as other measurements such as robot positon, which was were not used as a features in the model.
As can be seen on the attached ilustration during partial overlap peaks are visible in the sensor measurements (in certain directions). 
The goal was to train the model to those peaks/ anomalies.

<div align="center">
  <img src="https://github.com/danielstankw/Anomaly-Detection/assets/72759092/bce3bbdb-8464-4b58-8465-2b4cad63a923" width="700">
</div>

## Model (LSTM-Autoencoder)
The model used for this task was an LSTM Autoencoder. 
LSTM is a Neural Network capable of modeling short and long term dependanceies in data, therefore its use for time series data is justified. 
The strucutre of the network is presented below, and is implemented in Tensorflow.
The time series data is preprocessed by using windowing as well as applying moving average over the time series, next the data is feed into the Encoder part of the model which learns the compressed representation of the data. In the next step Decoder structures in exact same way as Encoder is used to decode the signal.

<div align="center">
  <img src="https://github.com/danielstankw/Anomaly-Detection/assets/72759092/a368b454-b62c-4cdc-978f-f4b7d294b79c" width="700">
</div>


## Training and Testing of the Model.
![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/76da597b-aada-4bb3-a6eb-d394ba605e39)
## Results
![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/1b225097-e5f3-4d85-90a9-a2e2e42264f1)

![image](https://github.com/danielstankw/Anomaly-Detection/assets/72759092/5c865cc1-ad2b-4de5-9bff-247bef43a14b)

# [The-GhostCar-An-Autonomous-Car-Project]()

## AIM
The Aim of this Project was to build a Fully Autonomous Car Simulation using Behavioural Cloning on Convolution Neural Networks Model.
<br>

## MOTIVATION
Autonomous cars are a boon for the vision of a smart world. Tesla, BMW, Google, NVIDIA are some of the companies contributing to this technology and have overcome major milestones in developing autonomous vehicles. With the development of autonomous cars, they can cause a huge boost to the transportation and automobile industries and hence we aimed to contribute to the Autonomous Car Development Industry. <br>
<br>

## CONTENTS
1) Drive.py - The Python Program hosts a Flask server on Local host to communicate controls to the simulation softwares. <br>
2) Behavioural Cloning.ipynb - Python Notebook File that shows the procedure and methods developed and used in order to build and train the CNN Model for the Autonomous Car. <br>
3) Model.h5 - Weights file for several trained models. <br>
<br>

## MODELS <br>
1) model1.h5 - Trained over 4053 samples and gives a loss of 0.0743 <br>
2) model2.h5 - Trained over 8205 samples and gives a loss of 0.369 <br>
3) model3.h5 - (Best) Trained over 30227 samples and gives a loss of 0.0276 <br>
<br>

<hr>
#Summary of the Design CNN Model
<br>
This Model is as per the Precribed [Nvidia Autonomous Driving Documentation](https://images.nvidia.com/content/tegra/automotive/images/2016/solutions/pdf/end-to-end-dl-using-px.pdf) <br>
_________________________________________________________________ <br>
Layer (type)                 Output Shape              Param #    <br>
================================================================= <br>
conv2d_21 (Conv2D)           (None, 31, 98, 24)        1824       <br>
_________________________________________________________________ <br>
conv2d_22 (Conv2D)           (None, 14, 47, 36)        21636      <br>
_________________________________________________________________ <br>
conv2d_23 (Conv2D)           (None, 5, 22, 48)         43248      <br>
_________________________________________________________________ <br>
conv2d_24 (Conv2D)           (None, 3, 20, 64)         27712      <br>
_________________________________________________________________ <br>
conv2d_25 (Conv2D)           (None, 1, 18, 64)         36928      <br>
_________________________________________________________________ <br>
flatten_5 (Flatten)          (None, 1152)              0          <br>
_________________________________________________________________ <br>
dense_17 (Dense)             (None, 100)               115300     <br>
_________________________________________________________________ <br>
dense_18 (Dense)             (None, 50)                5050       <br>
_________________________________________________________________ <br>
dense_19 (Dense)             (None, 10)                510        <br>
_________________________________________________________________ <br>
dense_20 (Dense)             (None, 1)                 11         <br>
================================================================= <br>
Total params: 252,219 <br>
Trainable params: 252,219 <br>
 <br>
<hr>

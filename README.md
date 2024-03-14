# CarPlateDetector

### Car Plate Identification Script for Security Cameras

This script uses a deep learning object detection model that was trained with [**custom car plate data**](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection).

## Usage

### Installing dependencies

Before running the script

    pip install -r requirements. txt

### Running the script

In order to run the script, initialize the server:

    python3 server/server.py

Then it will ask you for what camera it program shall use. After selecting the desired one, the script will start to run and a window will pop up with  the camera output. From then on, if the model recognizes a car plate, it will plot it and describe what's its confidence on it being a plate.

## Model

The used model was trained by transfering knowledge from another model. Then from that point onwards it was custom trained with [**this dataset**](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection) using only 2000 steps to train it. In the future I will train it further in order to improve its performance

The [**jupyter notebook**](https://github.com/joaodrmacas/carPlateDetector/model/CarPlateDetector.ipynb) explains how to setup the model training with steps to follow.

## Examples





## Performance tests

### **TODO:**

- Implement OCR to be able to save car plates onto the database
- Test performance and plot the results by checking if the script outputs the correct license plate characters

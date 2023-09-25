# A workflow for first floor line and ground line detection

## Introduction

This repository contains the resource code used by the authors for data preparation, training and testing the workflow of first floor line and ground line detection.

Code for data processing is in the folder `data_process`

Training weights avaliable is in the folder `weights`

`flow.ipynb` is about the whole flow of this process

If you want to train the detetction part of this flow, run `train_yolo8.ipynb`

## Usage in Colab

### Get the first line and ground line of your image

Step1: open `flow.ipynb` in colab

Step2: change the `.pt` path (saved model weights for detection part) and the image folder path based on your dataset

**NOTE:** If you do not want to finetune yolov8 using your own dataset, you can download the model weights saved in the folder `weights`. `best.pt` is recommended.

Step3: run the code and get both visualization results and txt results (records of the starting point and the end point of the line)


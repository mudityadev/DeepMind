# Deepfake-Videos-Detection-And-Generator
### Table of Contents

1.Overview - About The Project

2.Tools and Technique

3.Pipeline

4.How to Run

5.Environment Setup

6.Installation of Libraries

7.Command on Terminal

8.More Screenshots

9.Possible Improvements

10.Contact

### Overview - About The Project

## Deepfake Detection

<img width="1324" alt="model11" src="https://user-images.githubusercontent.com/60814715/138684329-a9df2ee2-e479-4860-980a-3e7f9355c1e6.png">
<img width="1325" alt="model1" src="https://user-images.githubusercontent.com/60814715/138684341-4fb3bcad-9862-4ae8-baab-115f57dc34cc.png">



We show that the model proposed in current state of the art in video manipulation (FaceForensics++) does not generalize to real-life videos randomly collected from Youtube.

We show the need for the detector to be constantly updated with real-world data, and propose an initial solution in hopes of solving deepfake video detection.

Our Pytorch implementation, conducts extensive experiments to demonstrate that the datasets produced by Google and detailed in the FaceForensics++ paper are not sufficient for making neural networks generalize to detect real-life face manipulation techniques. It also provides a current solution for such behavior which relies on adding more data.


## Deepfake Generator 

![epochs](https://user-images.githubusercontent.com/60814715/138685089-4fbce74d-2902-4b17-9e8e-5690993de831.gif)

Python notebook containing TensorFlow DCGAN implementation. It was trained on a Celebrities dataset.

### Tools and Technique
- Face Forensics++
- Phoneme-Viseme Mismatches
- Forensic Technique Using Facial Movements
- Recurrent Convolutional Strategy
- Celeb-DF
- Deepfakes detection challenge by Facebook, Microsoft 
- DeepfakeTIMIT
- Kaggle Deepfake Detection Challenge


### Pipeline

- Import all library - NumPy, OpenCV, Matplotlib

- Image Images

- Convert RGB image to Grayscale image

- Using Canny Edge detection

- Region of Interest - 4 Sided polygon to Mask

- Hough Transform

- Draw the lines

- Output


### How to Run

1.Ubuntu 20.04 or 18.04 (Environment)

2.Clone the repo

3.git clone

 - https://github.com/rmuditya/Lane-Line-Detection-for-Autonomous-Car-Truck-on-Images-Video.git 

4.Install Requirements

- pip3 install -r requirements

5.Open Terminal and Open Juypter

- juypter notebook

### Hardware Requirement

- Mostly trained on devbox configuration with 4xTitan V, thanks to Nvidia and DSB2018 competition where I got these gpus https://www.kaggle.com/c/data-science-bowl-2018/

- Overall training requires 4 GPUs with 12gb+ memory. Batch size needs to be adjusted for standard 1080Ti or 2080Ti graphic cards.

- As I computed fake loss and real loss separately inside each batch, results might be better with larger batch size, for example on V100 gpus. Even though SyncBN is used larger batch on each GPU will lead to less noise as DFDC dataset has some fakes where face detector failed and face crops are not really fakes.


### Possible Improvements

1.Proccessing for multiple images in a single run.

2.Speed of processing.

3.Details of the videos.


### Contact

Muditya Raghav

- Muditya Raghav
- Linkedin
- Twitter
- Instagram
- Gmail - rmuditya@gmail.com

### Codes

https://github.com/deepfakes/faceswap
https://github.com/dessa-oss/DeepFake-Detection

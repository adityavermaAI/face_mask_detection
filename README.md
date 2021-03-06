# Face Mask Detection and Record Keeping System

<p align="center">
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#about-the-project">View Demo</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Report Bug</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Request Feature</a>
</p>

<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li><a href="#about-the-project">About The Project<a></li>
    <li><a href="#procedure">Procedure</a></li>
    <li><a href="#dataset">Dataset</a></li>
    <li><a href="#image-Processing">Image Processing</a></li>
    <li><a href="#model">Model</a></li>
    <li><a href="#training">Training</a></li>
    <li><a href="#evaluation">Evaluation</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About The Project

In this project, I made a face mask detection system which detects whether the person is wearing a mask or not. If person without mask is detected then a face recognition system identifies the person and the necessary data like name of that person, date, time is saved in a database for further analysis.

![face_mask_demo 480](https://user-images.githubusercontent.com/72017583/115714561-dd680080-a394-11eb-8b76-c04c9687acf5.gif)

I also made an interactive Power Bi dashboard to show the trends in the data stored by the system. This dashboard can be accessed from anywhere, anytime through online services. This data is refreshed every second to show the live changes in the data.

![Face_mask_bi](https://user-images.githubusercontent.com/72017583/115701276-3f206e80-a385-11eb-908a-25b18b091bb0.gif)

## Procedure

Figure below shows the Block diagram of the procedure followed in this project.

![image](https://user-images.githubusercontent.com/72017583/115590219-595b3d80-a2ee-11eb-80d0-eb1f25e9fd20.png)

## Dataset

Data from two different sources are collected for training and testing the model. We collected a total of about 2000 images of people with masks and about 2000 images of people without a mask. For training purposes, 90% images of each class are used and the rest of the images are utilized for testing purposes. Figure. 3 shows some of the images of two different classes.

![image](https://user-images.githubusercontent.com/72017583/115589201-3419ff80-a2ed-11eb-8cec-09da9e274be4.png)


## Image Processing

The images captured by the cameras required preprocessing before going to the next step. In the preprocessing step, the image is transformed into a grayscale image because the RGB color image contains so much redundant information that is not necessary for face mask detection. RGB color image stored 24 bit for each pixel of the image. On the other hand, the grayscale image stored 8 bit for each pixel and it contained sufficient information for classification. Then, we reshaped the images into (100×100) shape to maintain uniformity of the input images to the architecture. Then, the images are normalized and after normalization, the value of a pixel resides in the range from 0 to 1. Normalization helped the learning algorithm to learn faster and captured necessary features from the images.


## Model

Figure below shows the architecture of the model used in this project.

![image](https://user-images.githubusercontent.com/72017583/125159763-0d09f600-e197-11eb-92ba-42a1e92ebd98.png)

## Training

In Figure below, the accuracy curve of training and testing is shown for about 5 epochs. From figure, it is realized that the training and testing accuracy are almost identical. This means the model has a decent generalization ability for previously unseen data and it does not cause overfitting of the training data.

![image](https://user-images.githubusercontent.com/72017583/115590693-e30b0b00-a2ee-11eb-8c6f-a58f60a8d9d2.png)

## Evaluation

In the figure below, we can see that the developed architecture misclassifies only 14 samples out of 381 samples. It classifies 5 sample as with mask while it is in without mask class and classifies 9 samples as without mask while these were in with mask class.

![image](https://user-images.githubusercontent.com/72017583/115590778-fae28f00-a2ee-11eb-9e42-e2e5651574c8.png)

Figure below shows that the system has very good precision and recall score as well as good accuracy.

![image](https://user-images.githubusercontent.com/72017583/115590922-29f90080-a2ef-11eb-94a1-a4cf221a84a3.png)


## Contact

E-Mail - adityaverma.ml@gmail.com

LinkdIn - [www.linkedin.com/in/adityavermaai](https://www.linkedin.com/in/adityavermaai)

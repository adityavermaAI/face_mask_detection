# Audio Event Detection using CNN

<p align="center">
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://user-images.githubusercontent.com/72017583/114261809-58770180-99fa-11eb-94d8-6144e3da168e.mp4">View Demo</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Report Bug</a>
    ·
    <a href="https://github.com/adityavermaAI/Audio-Event-Detection/issues">Request Feature</a>
</p>

<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li><a href="#about-the-project">About The Project<a></li>
    <li><a href="#Dataset">Dataset</a></li>
    <li><a href="#Model">Image Processing</a></li>
    <li><a href="#Training">Procedure</a></li>
    <li><a href="#Evaluation">Evaluation</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About The Project


Face mask detection is a technique to find out whether someone is wearing a mask or not. It is similar to detect any object from a scene.

![Face_mask_bi](https://user-images.githubusercontent.com/72017583/115701276-3f206e80-a385-11eb-908a-25b18b091bb0.gif)


## Dataset

Data from two different sources are collected for training and testing the model. We collected a total of about 2000 images of people with masks and about 2000 images of people without a mask. For training purposes, 90% images of each class are used and the rest of the images are utilized for testing purposes. Figure. 3 shows some of the images of two different classes.

![image](https://user-images.githubusercontent.com/72017583/115589201-3419ff80-a2ed-11eb-8cec-09da9e274be4.png)

## Image Processing

The images captured by the cameras required preprocessing before going to the next step. In the preprocessing step, the image is transformed into a grayscale image because the RGB color image contains so much redundant information that is not necessary for face mask detection. RGB color image stored 24 bit for each pixel of the image. On the other hand, the grayscale image stored 8 bit for each pixel and it contained sufficient information for classification. Then, we reshaped the images into (100×100) shape to maintain uniformity of the input images to the architecture. Then, the images are normalized and after normalization, the value of a pixel resides in the range from 0 to 1. Normalization helped the learning algorithm to learn faster and captured necessary features from the images.



## Procedure

Figure below shows the Block diagram of the procedure followed in this project.

![image](https://user-images.githubusercontent.com/72017583/115590219-595b3d80-a2ee-11eb-80d0-eb1f25e9fd20.png)

## Model

Figure below shows the architecture of the model used in this project.

![image](https://user-images.githubusercontent.com/72017583/114194765-6e8ab080-996d-11eb-84bb-700caacddccb.png)

## Evaluation

![image](https://user-images.githubusercontent.com/72017583/115590778-fae28f00-a2ee-11eb-9e42-e2e5651574c8.png)

![image](https://user-images.githubusercontent.com/72017583/115590922-29f90080-a2ef-11eb-94a1-a4cf221a84a3.png)

![image](https://user-images.githubusercontent.com/72017583/115590693-e30b0b00-a2ee-11eb-8c6f-a58f60a8d9d2.png)


## Contact

E-Mail - adityaverma.ml@gmail.com

LinkdIn - [www.linkedin.com/in/adityavermaai](https://www.linkedin.com/in/adityavermaai)

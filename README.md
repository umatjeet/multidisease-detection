[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555

<!-- PROJECT LOGO -->

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Table of Contents](#table-of-contents)
- [About The Project](#about-the-project)
  - [Steps involved](#steps-involved)
  - [Tools used](#tools-used)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Data Analysis and Model Building](#data-analysis-and-model-building)
  - [Application Development](#application-development)
- [Usage](#usage)
- [Contact](#contact)

<!-- ABOUT THE PROJECT -->

## About The Project

<p align="center">
  
</p>
This project uses <a href="https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia">Chest X-Ray dataset</a> from kaggle.
The dataset is organized into 3 folders (train, val & test) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal). These images are used for building an CNN model using keras to detect pneumonia in patients based on X-ray reports.For malaria dataset we have used <a href=https://lhncbc.nlm.nih.gov/">malaria dataset</a>. Malaria dataset has two catagories parasitized and uninfected. We also used cnn for training model for malaria detection. After model building the best performing model is used to build a flask base web application.

### Steps involved

- Reading data from source and preprocessing it using OpenCV.
- Performing data preprocessing before feeding the data to the model.
- Building sequential model architecture using keras.
- Using data augmentating to prevent the model from overfitting during training phase.
- Creating web application using flask to detect Pneumonia upon receiving the preprocessed X-ray.

### Tools used

Following are the tools/frameworks used in developing the application:

- [CSS](https://en.wikipedia.org/wiki/CSS)
- [Python](https://www.python.org/)
- [Flask](https://palletsprojects.com/p/flask/)
- [HTML](https://en.wikipedia.org/wiki/HTML)
- [OpenCV](https://opencv-python-tutroals.readthedocs.io/en/latest/)

## Getting Started

### Installation

For proper execution of application firstly create an environment, then to install prerequisite libraries execute below command in terminal.

```
pip install -r requirements.txt
```

### Data Analysis and Model Building

Refer `Pneumonia_Detection_CNN.ipynb` to find details regarding data analysis and model building.

Since this is a classification problem, to check model performance `Confusion Matrix` and `Classification Report` are used.

<p align="center">
<b>Confusion Matrix</b><br>
<img src="https://raw.githubusercontent.com/rppradhan08/pneumonia-detection/master/images/cunfusion_mat.png" height="200px">
</p>

### Application Development

After model development, the web application is developed using `flask` which is a python based web-framework. For source code refer `app.py`.

Below are few snapshots of application in use:

- Step 1 Uploading X-Ray
  <p align="center">
    <img src="https://github.com/umatjeet/pneumonia-detection/blob/main/images/home.png" height="300px">
  </p>
- Step 2 Displaying Result
  <p align="center">
    <img src="https://github.com/umatjeet/pneumonia-detection/blob/main/images/normal.png" height="200px">
  </p>

<!-- CONTACT -->

## Usage

To run this application firstly execute `python app.py`, after which the flask built-in server would start hosting the application at localhost i.e.
`http://127.0.0.1:5000/`

## Contact
Jeet Umat - 201801231@daiict.ac.in
Ajay Vala - 201801414@daiict.ac.in
Hardik Madhwani - 201801409@daiict.ac.in


# Emotion-Based Music Player

A web-based music player which detects the user's mood and recommends a set of songs, while changing its background theme accordingly. Made using HTML/CSS/Javascript for the frontend and Django/Python for the backend. The backend integrates both the Haar Cascade machine learning model and a CNN classifier through OpenCV. The classifier was trained using Colaboratory and Tensorflow. Essentially, the Haar Cascade algorithm utilizes the user's webcam to locate the user's face, which is then passed onto the classifier to detect what emotion the person is displaying. The classifier is trained on 4 emotions: Angry, Happy, Calm, and Sad. Depending on what emotion it detects, it will change the song selection and background of the music player accordingly.

### Prerequisites

See requirements.txt.

```
tensorflow-cpu
opencv-python-headless
Django==3.1.2

#### Demonstration

Deployed on Heroku: https://emotion-music-player.herokuapp.com/

##  Used Technologies

* HTML/CSS - Frontend styling and web page design
* Javascript - Frontend music player functions
* Django - Backend integration of machine learning algorithms
* OpenCV - Computer vision tasks
* Colab/Tensorflow - Training the emotion classifier

### Dataset

The dataset was initially retrieved from Kaggle from a <a href="https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data">research prediction competiton</a> titled "Challenges in Representation Learning: Facial Expression Recognition Challenge." A <a href="https://drive.google.com/drive/folders/1bCFKTkmItIZl73YNUq5QXppLpIdmTgUv">direct link</a> to the dataset is also provided. The data consists of 48x48 pixel grayscale images of faces. The faces have been automatically registered so that the face is more or less centered and occupies about the same amount of space in each image. Even though there are 7 labelled classes of expressions, we only decided to utilize the 4 most common ones.

### Training Results

Final Accuracy = 58.33%, Validation Accuracy = 54.99%


# Gauge
An app for teachers to gauge student understanding in online learning platforms. 

I came up with the idea during the pandemic lockdown when I observed the challenges my teachers faced teaching virtually. I presented this concept it at the HackDuke2020: Code for Good where it won 3rd Place. 

This repo contains code for a convoluted neural network (CNN) that detects the seven universal facial expressions. [Anger, Disgust, Fear, Happiness, Neutral, Sadness, Fear].

This neural network plays an essential role in Gauge. Gauge is a zoom add-on that allows teachers to better understand how their students are learning the content being taught. The app uses this facial expression model to determine if the students are confused/don’t understand the content and based on that, alert the teacher.

Facial_Expression_Training.py contains code that creates multiple layers of the neural network and trains it on of images of all kinds of facial expressions.

Camera.py contains code for analyzing expressions in video feeds using a facial detection model that puts a bounding box around a person’s face.

Model.py uses the trained model along with its weights to develop predictions when given an image/video feed.

The test folder contains images used for validation and testing

I compared this approach with retraining (using transfer learning) the google inception model and presented my results at the 2021 Sysnopsys Science Fair. It won 1st Place in the Physical Sciences and Engineering Category. The slides and video demo for the entire project are here.

Slides:https://docs.google.com/presentation/d/1aRpopFNNnE-30FYAl1hSQEFcmB8Vcuv83PvV8kEJBDg/edit?usp=sharing

Video Demo: https://youtu.be/D36C48vVtdM

Credit to https://www.coursera.org/projects/facial-expression-recognition-keras for the tutorial.

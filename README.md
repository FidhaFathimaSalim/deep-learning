# Computer Vision & Deep Learning Basics

This repository contains a collection of Python scripts demonstrating various computer vision, deep learning, and image processing techniques. These scripts are categorized into progressive "Days", showing different applications of popular libraries like OpenCV, MediaPipe, and DeepFace.

## 🚀 Projects Overview

Here is a breakdown of the daily scripts included in this repository:

### Day 1: Basics & Emotion Recognition
*   **`day_1.py`**: A simple starter script to practice opening the webcam and capturing video streams using OpenCV.
*   **`day_1_emotion.py`**: Live facial emotion recognition using the `deepface` library to analyze the webcam feed and detect the dominant emotion.
*   **`day_1_speechemo.py`**: An advanced version of emotion recognition that integrates `pyttsx3` to audibly speak out the emotion it detects ("You look happy", etc.) using multithreading to avoid freezing the video stream.

### Day 2: Advanced Landmarks & Tracking
*   **`day_2.py`**: Implements basic face landmark tracking using `mediapipe.solutions.face_mesh` to map out facial key points in real-time.
*   **`day_2_hand.py`**: Hand tracking with MediaPipe, featuring real-time **distance estimation** of your hand from the camera by calculating perceived width compared to a known focal length.

### Day 3: Cool Applications & Pose Estimation
*   **`day_3.py`**: Extends Day 2 by creating a tessellation mask over tracked face landmarks.
*   **`day_3_color.py`**: A color filtering script that isolates the color red from the webcam feed using HSV color spaces.
*   **`day_3_invisible_cloak.py`**: The classic "Harry Potter Invisibility Cloak" trick! It detects red objects in the frame and replaces them with a pre-saved background image.
*   **`day_3_personal_trainer.py`**: An AI personal trainer that tracks arm movement during a dumbbell curl exercise. It automatically counts your repetitions and calculates the curl percentage mapped visually to a bar.
*   **`PoseModule.py`**: A custom, reusable Python class wrapping MediaPipe's Pose functionality. It is utilized in the personal trainer app to extract pose landmarks and calculate anatomical joint angles seamlessly.

## 🛠 Prerequisites & Installation

To run the scripts in this repository, you will need a computer with a webcam and **Python 3.9.13** (the version used during development). 

1. Ensure Python 3.9.13 is installed on your system.
2. Install the required dependencies using pip:

```bash
pip install opencv-python mediapipe deepface pyttsx3 numpy
```

## 🎮 How to Run
Navigate precisely to the directory containing the scripts and run any file using python:
```bash
python day_3_invisible_cloak.py
```
*(Tip: For scripts like `day_3_invisible_cloak.py`, give the camera a few seconds to capture the clean background before stepping into the frame with your "cloak").*
Press **`q`** on your keyboard to quit the webcam feed and close any running script.

## 💡 Technologies Used
*   **[OpenCV](https://opencv.org/)**: Video capturing, image processing, and rendering.
*   **[MediaPipe](https://google.github.io/mediapipe/)**: Face, Hands, and Pose high-fidelity landmark tracking.
*   **[DeepFace](https://github.com/serengil/deepface)**: State-of-the-art framework for emotion and facial analysis.
*   **pyttsx3**: Offline Text-to-Speech conversion.

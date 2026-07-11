# Drowsiness Detection System

A real-time computer vision system to detect driver drowsiness using webcam input, built to understand image processing and deep learning concepts for driver safety applications.

## Overview
This project trains a deep learning model on a 2-class dataset (drowsy / alert) and uses it for real-time detection through webcam feed. Haar Cascade classifiers are used for face and eye detection, combined with the trained model to classify drowsiness state.

## Tech Stack
- Python
- TensorFlow / Keras
- OpenCV
- Haar Cascade Classifiers (face & eye detection)

## Project Structure
```
├── DATASET/                  # Training dataset (awake / sleepy classes)
├── DROWSINESS_DETECTION.ipynb   # Model training notebook
├── drowsiness_model.h5        # Trained model
├── haarcascade_frontalface_default.xml   # Face detection classifier
├── haarcascade_eye_tree_eyeglasses.xml   # Eye detection classifier
└── images/                   # Sample images
```

## How It Works
1. Face and eyes are detected in real-time from webcam feed using Haar Cascade classifiers.
2. The trained CNN model classifies the eye/face region as "drowsy" or "alert."
3. An alert is triggered if drowsiness is detected continuously.

## Approach
- Trained a model on a 2-class dataset (drowsy / alert) sourced from labeled driver images.
- Used Haar Cascade classifiers for face and eye region detection.
- Tested the system in real-time using webcam input to validate detection accuracy.

## Results
*(Add your model's accuracy/performance metrics here)*

## Future Improvements
- Add sound-based alert system for real-time warnings
- Improve accuracy with a larger, more diverse dataset
- Deploy as a lightweight application for in-vehicle use

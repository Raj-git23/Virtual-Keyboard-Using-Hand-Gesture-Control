# Hand Gesture Typing System - README

## Overview
This project implements a hand gesture-based typing system using a webcam, Mediapipe for hand tracking, OpenCV for visual feedback, and Pynput for simulating keyboard inputs. The system detects hand gestures, such as hovering over keys and making specific finger movements, to simulate typing on a virtual QWERTY keyboard.

## Features

*   **Real-time Hand Tracking**: Uses Mediapipe to detect and track 21 hand landmarks, enabling precise hand and finger position recognition.
*   **Virtual Keyboard**: A QWERTY keyboard is drawn on the screen, where each key can be clicked using hand gestures.
*   **Gesture Recognition**: Recognizes "click" gestures by calculating the distance between the index and middle fingertips.
*   **Keyboard Simulation**: Uses the Pynput library to simulate real keyboard inputs, enabling text entry in any active application.
*   **Visual Feedback**: Displays typed text in real-time, providing immediate feedback to users.

## Requirements

Before running the code, ensure you have the following dependencies installed:

*   Python 3.x
*   OpenCV
*   Mediapipe
*   Numpy
*   Pynput

You can install the required libraries using the following commands:

```bash
pip install opencv-python mediapipe numpy pynput


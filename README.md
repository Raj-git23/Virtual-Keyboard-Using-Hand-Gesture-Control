Hand Gesture Typing System - README
Overview
This project implements a hand gesture-based typing system using a webcam, Mediapipe for hand tracking, OpenCV for visual feedback, and Pynput for simulating keyboard inputs. The system detects hand gestures, such as hovering over keys and making specific finger movements, to simulate typing on a virtual QWERTY keyboard.

Features
Real-time Hand Tracking: Uses Mediapipe to detect and track 21 hand landmarks, enabling precise hand and finger position recognition.
Virtual Keyboard: A QWERTY keyboard is drawn on the screen, where each key can be clicked using hand gestures.
Gesture Recognition: Recognizes "click" gestures by calculating the distance between the index and middle fingertips.
Keyboard Simulation: Uses the Pynput library to simulate real keyboard inputs, enabling text entry in any active application.
Visual Feedback: Displays typed text in real-time, providing immediate feedback to users.
Requirements
Before running the code, ensure you have the following dependencies installed:

Python 3.x
OpenCV
Mediapipe
Numpy
Pynput
You can install the required libraries using the following commands:

bash
Copy code
pip install opencv-python mediapipe numpy pynput
How It Works
Camera Capture: The system uses your webcam to capture video frames in real-time.
Hand Tracking: Mediapipe detects and tracks the positions of your hands and fingers, drawing landmarks and connections on the screen.
Virtual Keyboard: A virtual QWERTY keyboard layout is displayed on the screen. Each key is represented as an interactive button.
Gesture Recognition: When your index and middle fingers hover over a key and come close to each other (within a defined distance), a "click" is simulated.
Keyboard Simulation: When a key is clicked, the corresponding character is sent as a keyboard input, which is displayed in real-time on the screen.
Usage
Run the script.
The webcam will activate, and you will see a virtual keyboard on the screen.
Hover your hand over the keyboard and bring your index and middle fingers close together to "click" on the keys.
The typed text will be displayed in real-time in a text box.
To exit the program, press the 'Q' key.
Code Structure
Imports: Imports necessary libraries such as OpenCV, Mediapipe, Numpy, and Pynput.
Button Class: Defines a class to represent individual keys on the virtual keyboard.
Draw Functions: Functions to draw the virtual keyboard and interact with hand landmarks.
Distance Calculation: Function to calculate the distance between the index and middle fingertips to detect click gestures.
Main Loop: The main loop processes video frames, detects hand landmarks, recognizes gestures, and simulates keyboard input.
Example
Once the script is executed, you will see the webcam feed with the virtual keyboard displayed. As you move your hand over the keys and perform gestures, the corresponding characters will appear in the text box.

Troubleshooting
Low Accuracy or Performance: Ensure your webcam is working properly and the lighting conditions are sufficient for hand detection.
Slow Response: The system may slow down if the system resources are heavily utilized or if the webcam resolution is too high. Try adjusting the resolution by modifying cap.set(3, 1280) and cap.set(4, 720).
License
This project is open-source and free to use. Feel free to modify and improve it as needed!

By following the above steps and utilizing this README, users can understand the project, install necessary dependencies, and utilize the hand gesture typing system.

# Fingers Counter

## Project Overview
The primary objective of this project is to develop an interactive system that combines an Arduino Uno microcontroller, LEDs, and a 7-segment LCD display. The system is controlled and monitored using Python to enable real-time data visualization and control.

## Design Overview
### Hardware Components
- **Arduino Uno**: The core microcontroller managing LED and 7-segment display operations.
- **LEDs**: Visually represent the number of fingers detected.
- **7-Segment LCD Display**: Displays the numeric count of fingers detected.
- **Laptop Camera**: Captures real-time images for processing.

### Software Components
- **Python**: Implements the image processing algorithm for finger detection and sends the detected count to the Arduino.
- **OpenCV Library**: Used for image processing tasks, such as detecting and counting fingers.
- **Arduino IDE**: Contains the program logic for controlling the hardware based on input received from Python.

## Algorithms Used
### 1. Image Processing Algorithm
1. Capture video feed from the camera.
2. Preprocess the image.
3. Detect the hand region using contour detection.
4. Analyze the hand contour to count the number of fingers raised using convex hull and defect detection techniques.

### 2. Logical Operations
- Map the detected number of fingers to the number of LEDs to be activated.
- Convert the detected number into a format compatible with the 7-segment display.

This project effectively demonstrates the integration of hardware and software to create an interactive, real-time finger counting system.


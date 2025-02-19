# Fingers Counter

## Explaining The Design:
The primary objective of this project was to develop an interactive system combining an
Arduino Uno microcontroller, LEDs, and a 7-segment LCD display, controlled and
monitored using Python programming language. This project demonstrates efficient
communication between hardware and software for real-time data visualization and
control.


## Design Overview:
*1- Hardware:*
Arduino Uno: The core microcontroller managing LED and 7-segment display operations
LEDs: Used to visually represent the number of fingers detected
7-Segment LCD Display: Displays the numeric count of fingers detected
Laptop Camera: Serves as the input device for capturing images in real-time
*2- Software:*
Python: Implements the image processing algorithm for finger detection and sends the
detected count to the Arduino
OpenCV Library: Used for image processing tasks, such as detecting and counting fingers
Arduino IDE: Contains the program logic for controlling the hardware based on the input
received from Python

## Algorithms Used:
*1- Image Processing Algorithm:*
Capture video feed from the camera Preprocess the image
Detect the hand region using contour detection
Analyze the hand contour to count the number of fingers raised using convex hull and
defect detection techniques
*2- Basic Logical Operations:*
Map the detected number of fingers to the number of LEDs tobe activated
Convert the number into a format compatible with the 7-segment display
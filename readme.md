## Domain: 
Computer Vision 

## Title of the project:
 Operating Computer Cursor using Eye and Face movements 

## Abstract: 
The advent of modern human computer interfaces has seen a considerable progress in 
Handsfree Human Computer Interaction (HCI) solutions. This project focuses on developing 
a methodology to facilitate computer cursor control for people with physical disabilities such 
as Quadriplegics and amputees. An innovative solution for individuals facing physical 
challenges in using a traditional mouse by introducing eye gaze control for the mouse cursor. 
Opening/closing the mouth based on Mouth Aspect Ratio (MAR) indicates 
activation/deactivation of the cursor control. The nose tip is used for controlling and moving 
the cursor in all 4 directions by moving the head left, right, up and down. Eye Aspect Ratio 
(EAR) is used to detect eyes and eye flickering. Left and right eye blinks indicate left and right 
clicks respectively. Squinted eyes indicate scrolling of pages, which is beneficial while 
working with PDFs and other such documents. The proposed system requires very basic 
requirements like webcam and a few Python libraries such as OpenCV, Numpy, imutils, dlib 
and PyAutoGUI. This alternative method leverages eye movements, catering to those who find 
touchscreens or traditional mice inaccessible. The system, implemented in Python by using 
OpenCV library, tracks both iris movement and cursor positioning, providing an efficient and 
user-friendly virtual mouse controller accessible to anyone, especially those with physical 
disabilities relying on eye movements.
Keywords:- Eye Tracking, Virtual Mouse, web-cam based interaction, Human-computer 
interaction, OpenCV, 68point landmark algorithm, MAR, EAR.

## Code Requirements:
Numpy
OpenCV
PyAutoGUI
Dlib
Imutils
Utils

## Functionalities:
* Eye Gaze Control: Utilizing eye movements to control the computer cursor, enabling handsfree interaction.
* Mouth Activation: Opening and closing the mouth triggers the activation and deactivation of cursor control, facilitating seamless transitions.
* Head Movement Control: Using the nose tip and head movement to navigate the cursor in four directions: left, right, up, and down.
* Eye Blink Detection: Detecting left and right eye blinks to perform left and right clicks respectively, enhancing user interaction.
* Eye Flickering Detection: Monitoring eye flickering, specifically for indicating scrolling actions, particularly useful for document navigation.
* Integration with Python Libraries: Leveraging Python libraries including OpenCV, NumPy, imutils, dlib, and PyAutoGUI for implementation and functionality.
* Accessibility: Catering to individuals with physical disabilities by providing an alternative, accessible method for cursor control through eye movements.

## Dependencies:
* Hardware: 
Basic webcam for capturing facial movements and eye gestures.
* Software:
Python programming language for system implementation.
OpenCV for computer vision tasks including facial recognition and eye tracking.
NumPy for numerical computing tasks.
imutils for image processing utilities.
dlib for facial feature detection and tracking.
PyAutoGUI for controlling the mouse cursor and simulating mouse clicks.
* Algorithm Development:
Development of algorithms for eye gaze tracking, mouth aspect ratio analysis, head movement detection, eye blink detection, and eye flickering detection.
* Testing and Optimization:
Rigorous testing to ensure accuracy, reliability, and user-friendliness of the system.
Optimization of algorithms and parameters to improve system performance and responsiveness.
* User Feedback and Iteration:
Incorporating user feedback to enhance system usability and address user needs.
Iterative development process to refine features and address potential issues.

## How to implement:
* Import all the required packages with proper versions
* Have all the required site packages installed in the system
* Check and adjust the treshold values
* shape_predictor_68_face_landmarks.dat file should be placed in model file and give correct path of the dat file in the code
* Run the code
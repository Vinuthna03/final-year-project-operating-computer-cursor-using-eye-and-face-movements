# OPERATING COMPUTER CURSOR USING EYE AND FACE MOVEMENTS

# ABSTRACT:
The advent of modern human computer interfaces has seen a considerable progress in Handsfree Human Computer Interaction (HCI) solutions. This project focuses on developing a methodology to facilitate computer cursor control for people with physical disabilities such as Quadriplegics and amputees. An innovative solution for individuals facing physical challenges in using a traditional mouse by introducing eye gaze control for the mouse cursor. Opening/closing the mouth based on Mouth Aspect Ratio (MAR) indicates activation/deactivation of the cursor control. The nose tip is used for controlling and moving the cursor in all 4 directions by moving the head left, right, up and down. Eye Aspect Ratio (EAR) is used to detect eyes and eye flickering. Left and right eye blinks indicate left and right clicks respectively. Squinted eyes indicate scrolling of pages, which is beneficial while working with PDFs and other such documents. The proposed system requires very basic requirements like webcam and a few Python libraries such as OpenCV, Numpy, imutils, dlib and PyAutoGUI. This alternative method leverages eye movements, catering to those who find touchscreens or traditional mice inaccessible. The system, implemented in Python by using OpenCV library, tracks both iris movement and cursor positioning, providing an efficient and user-friendly virtual mouse controller accessible to anyone, especially those with physical disabilities relying on eye movements.
Keywords: Eye Tracking, Virtual Mouse, web-cam based interaction, Human-computer interaction, OpenCV, 68point landmark algorithm, MAR, EAR.

# How the system works:
The innovative system for controlling the computer cursor using eye and facial movements represents a significant advancement in human-computer interaction. Here's a detailed elaboration on how the system works and the actions it enables:
1. Real-time Video Input with OpenCV: The system begins by capturing real-time video input using OpenCV (Open Source Computer Vision Library), a widely-used open-source library for computer vision and image processing tasks. This enables the system to continuously analyze the user's facial expressions and movements.
2. Face Detection with dlib's HOG Feature and Linear Classifier: Utilizing dlib's HOG feature combined with a linear classifier, an image pyramid, and a sliding window detection scheme, the system detects the user's face in the video stream. The Histogram of Oriented Gradients (HOG) feature descriptor is effective for object detection tasks, such as detecting faces, while the linear classifier helps classify the detected regions as faces.
3. Facial Landmark Detection with dlib's 68 Point Facial Landmark Detector: Once the face is detected, dlib's 68 point facial landmark detector is employed to pinpoint specific facial features crucial for action recognition. This detector identifies key landmarks on the face, such as the eyes, nose, mouth, and eyebrows, which are essential for interpreting the user's facial expressions and movements accurately.
4. Action Recognition using Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR): The system leverages the detected facial landmarks to recognize various actions performed by the user. For instance, a blink or wink is detected through the Eye Aspect Ratio (EAR), which measures the ratio of the distances between certain landmarks on the eye region. Similarly, a yawn can activate or deactivate controls using the Mouth Aspect Ratio (MAR), which indicates the openness of the mouth.

# Cursor Control Actions Enabled by the Proposed Algorithm:
The system offers a range of hands-free actions for controlling the computer cursor, including:
1. Squinting Eyes for Scroll Mode Activation
2. Winking for Left and Right Clicks
3. Head Movement (Pitch and Yaw) for Cursor Movement
4. Mouth Opening for Cursor Control Activation/Deactivation

# Code Requirements:
Coder Editor: Visual Studio Code
Language: Python
Packages:
1.Numpy
2.OpenCV
3.PyAutoGUI
4.Dlib
5.Imutils
6.Utils

# Dependencies:
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

# Functionalities:
* Eye Gaze Control: Utilizing eye movements to control the computer cursor, enabling handsfree interaction.
* Mouth Activation: Opening and closing the mouth triggers the activation and deactivation of cursor control, facilitating seamless transitions.
* Head Movement Control: Using the nose tip and head movement to navigate the cursor in four directions: left, right, up, and down.
* Eye Blink Detection: Detecting left and right eye blinks to perform left and right clicks respectively, enhancing user interaction.
* Eye Flickering Detection: Monitoring eye flickering, specifically for indicating scrolling actions, particularly useful for document navigation.
* Integration with Python Libraries: Leveraging Python libraries including OpenCV, NumPy, imutils, dlib, and PyAutoGUI for implementation and functionality.
* Accessibility: Catering to individuals with physical disabilities by providing an alternative, accessible method for cursor control through eye movements.

# How to implement:
* Import all the required packages with latest versions
* Have all the required site packages installed in the system
* Check and adjust the treshold values
* Create a model file. shape_predictor_68_face_landmarks.dat file should be placed in model file and give correct path of the dat file in the code
* Run the code

# REFERENCES
[1]V. Khare, S. G. Krishna and S. K. Sanisetty, "Cursor Control Using Eye Ball Movement," 2019 Fifth International Conference on Science Technology Engineering and Mathematics (ICONSTEM), 2019, pp.232- 235, doi: 10.1109/ICONSTEM.2019.8918780.
[2]Maruthapillai, Vasanthan & M, Murugappan & Nagarajan, R. & Ilias, Bukhari & Letchumikanth, J..(2012). Facial expression based computer cursor control system for assisting physically disabled person. Proceeding - COMNETSAT 2012: 2012 IEEE International Conference on Communication, Networks  and Satellite. 172-176. 10.1109/ComNetSat.2012.6380800.
[3]Mehta, Sukrit and Dadhich, Sharad and Gumber, Sahil and Jadhav Bhatt, Arpita, Real-Time Driver  Drowsiness Detection System Using Eye Aspect Ratio and Eye Closure Ratio (March 20, 2019). Proceedings of International Conference on Sustainable Computing in Science, Technology and  Management (SUSCOM), Amity University Rajasthan, Jaipur - India, February 26-28, 2019
[4]S. Mohanty, S. V. Hegde, S. Prasad and J. Manikandan, "Design of Real-time Drowsiness Detection  System using Dlib," 2019 IEEE International WIE Conference on Electrical and Computer Engineering (WIECON-ECE), 2019, pp. 1-4, doi: 10.1109/WIECON-ECE48653.2019.9019910.
[5]A. Rosebrock, Facial Landmarks with dlib, OpenCV, and Python, April 2017, Available: https://www.pyimagesearch.com/2017/04/03/facial-landmarks-dlib-opencv-python/
[6]How to detect eye blinking in videos using dlib and OpenCV in Python, June 2020, Available: http://datahacker.rs/011-how-to-detect-eye-blinking-in-videos-using-dlib-and-opencv-in-python/
[7]Relangi S.P.K., Nilesh M., Kumar K.P., Naveen A. (2020) Full Length Driver Drowsiness Detection Model—Utilising Driver Specific Judging Parameters. In: Reddy A., Marla D., Simic M., Favorskaya M., Satapathy S. (eds) Intelligent Manufacturing and Energy Sustainability. Smart Innovation, Systems and Technologies, vol 169. Springer, Singapore. https://doi.org/10.1007/978-981-15-1616-0

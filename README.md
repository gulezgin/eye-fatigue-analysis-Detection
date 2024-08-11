# eye-fatigue-analysis-Detection
This project is an eye blink detection application used to detect fatigue by tracking eye movements in a video stream.

Blink Detection and Fatigue Detection
This project is an application that detects users' fatigue by monitoring eye blink movements in the video stream. It detects fatigue using the eye's closing rate (Eye Aspect Ratio, EAR) and shows an alert on the screen.

Features
Face and eye detection
Calculating eye closure ratio (EAR)
Set a threshold value for fatigue detection
Show fatigue warning on screen
Requirements
Python 3.x
OpenCV
dlib
numpy
scipy
To install the required Python packages:

bash
copy code
pip install opencv-python dlib numpy scipy
Setup
Download Dlib's Face Point Model:

Download shape_predictor_68_face_landmarks.dat from dlib.net and place it in the project folder.

Run Your Code:

Run your Python script using the following command:

bash
copy code
python main.py
Code Description
calculate_ear(eye): Calculates the closing ratio of an eye.
draw_eye_landmarks(frame, eye_landmarks): Marks important points on the eye on the screen.
main(): Starts the video stream, detects face and eyes, calculates EAR and shows fatigue warning.
Use
After starting the application, images are taken with the webcam.
The closing rate of your eyes is monitored and when it is below the set threshold value, "FATIGUE DETECTED!" message appears on the screen.
Press q to exit the program.
Troubleshooting
Make sure the shape_predictor_68_face_landmarks.dat file is in the right place.
Check camera access permissions and make sure no other apps are using the camera.
Contributing
If you would like to contribute to this project, you can help by submitting a pull request or solving open issues

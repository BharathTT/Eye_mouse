# Eye_mouse
Eye-Controlled Mouse with Python and OpenCV

Title: Eye-Controlled Mouse

Description:
This Python script implements an eye-controlled mouse using computer vision and facial landmark detection. The script utilizes OpenCV (cv2) for image processing, Mediapipe for face landmark detection, and PyAutoGUI for mouse control.

The program captures video frames from the default camera (usually webcam) and processes them in real-time. It detects the user's face and identifies facial landmarks using Mediapipe's FaceMesh model. The specific facial landmarks corresponding to the eyes are then used to control the mouse cursor's movement.

The eye-tracking functionality relies on detecting changes in the vertical positions of certain facial landmarks associated with the eyes. By calculating the difference in vertical positions between these landmarks, the script determines whether the user is blinking or closing their eyes.

To move the mouse cursor, the script maps the eye landmark positions to the screen's resolution using PyAutoGUI. As the user blinks or closes their eyes, the mouse cursor moves accordingly.

Additionally, the script is designed to simulate a mouse click when the user blinks or closes their eyes for an extended duration, indicated by the distance between two specific eye landmarks being below a threshold value.

To run this script, ensure you have Python and the required libraries installed (cv2, mediapipe, and pyautogui). You can execute the script by simply running it in your Python environment.


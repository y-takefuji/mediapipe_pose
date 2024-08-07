# mediapipe_pose
Three programs (pose.py, posexy.py, and fposeservo.py) are disclosed.

In order to run the programs, you should install mediapipe by:

$ pip install mediapipe


If you have a problem on Windows 10: 

DLL load failed while importing _framework_binding

Run the following command on Windows 10.

$ pip install msvc-runtime

Three programs can show landmarks of a human body.

pose landmarks composed of 33 points are as follows:
<img src='https://github.com/y-takefuji/mediapipe_pose/blob/main/pose_tracking_full_body_landmarks.png' width=772 heigh=438>

source:https://developers.google.com/static/mediapipe/images/solutions/pose_landmarks_index.png

# pose.py
pose.py is a program to show 33 points of pose landmarks.

# posexy.py
posexy.py is a program to show 33 points of pose landmarks 
where nose coordinate(x,y) is displayed on the screen.

# fposeservo.py
fposeservo.py is a program working with Arduino firmata.
The nose coordinate (x,y) is equivalent to pose landmarks[0].
The horizontal nose x-axis with landmarks[0][0] controls a servo angle.

<img src='https://github.com/y-takefuji/mediapipe_pose/blob/main/nose.gif' width=320 heigh=240>

# Exercise

1. Nose position can turn LED on or off with firmata library.

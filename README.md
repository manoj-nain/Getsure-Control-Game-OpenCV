# Getsure-Control-Game-OpenCV
Gesture controlled Hill Climb Racing game using OpenCV, Python

**directkeys.py** has the code to control keyboard using ctypes library and scancodes. I am controlling left arrow and right arrow keys. If you need to control any other keys just add the hex code for those keys. Remember to turn Numlock if you are controlling arrow keys. I have taken some of this code from stackoverflow answer to this question: https://stackoverflow.com/questions/13564851/how-to-generate-keyboard-events-in-python.

**gesturecontrol.py** is our main file which has the code to detect color (yellow in my case) and control the keys accordingly. The idea is to take live feed rom the webcam then devide the frame in two parts at bottom. Bottom right area will control accelartion pedal (right arrow key) and left area will control brake pedal (left arrow key). Create a color mask and detect the contors in specfic areas. 


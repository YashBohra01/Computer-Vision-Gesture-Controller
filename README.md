# Computer-Vision-Gesture-Controller-
A project using Computer Vision to detect and track user's hand gestures with webcam input and controls system volume based on gestures. Implemented on Python 3 using Mediapipe. Developed for MacOS but can be easily implemented for Windows/Linux. Currently implemented for system volume but can easily be expanded to brightness, switching desktops on MacOS, etc using osascript.

Code detects position of tip of index finger and thumb, and varies system volume using osascript based on distance between the index finger and thumb. 

Tip of index finger and tip of thumb are 4th and 8th data points in hand landmark list returned from mediapipe findPosition() method. Refer to VolumeHandControl.ipynb

Note: VolumeHandControl.ipynb requires HandTrackingModule.ipynb file to run. VolumeHandControl.ipynb also has variable sliding of volume, but hardcoded mute, 50% and 100% volume only sliding can be implemented by uncommenting code in VolumeHandControl.ipynb.

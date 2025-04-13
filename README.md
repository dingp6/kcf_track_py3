# kcf_track_py3
This project is modified form [KCFpy](https://github.com/uoip/KCFpy) and (https://github.com/LCorleone/KCF_py3) can run with py3.
# Update
Fixed a bug that caused the program to crash when the tracking box became too small. 
# Requirements:
```shell
pip install -r requirements.txt 
```
* py3.6
* NumPy
* Numba (needed if you want to use the hog feature)
* OpenCV (ensure that you can import cv2 in python)

# Usage：
Download the sources and execute
```shell
git clone https://github.com/dingp6/kcf_track_py3.git
cd kcf_track_py3
python run.py
```
It will open the default camera of your computer, you can also open a different camera or a video
```shell
python run.py 1
```
```shell
python run.py ./test.avi  
```
Try different options (hog/gray, fixed/flexible window, singlescale/multiscale) of KCF tracker by modifying the arguments in line `tracker = kcftracker.KCFTracker(False, True, False)  # hog, fixed_window, multiscale` in run.py.

use your mouse to choose the roi 
press ESC to quit"# kcf_track_py3" 

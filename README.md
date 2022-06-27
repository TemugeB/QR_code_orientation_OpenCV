# QR code orientation using OpenCV

![Alt text](media/Example.gif?raw=true "Example output.")

Simple demo that uses OpenCV QR detector and photogrammetry functions to determine the location and orientation of QR code in camera view. Explanation of the code is provided as a blog post here: [link](https://temugeb.github.io/python/computer_vision/2021/06/15/QR-Code_Orientation.html). In this demo, I've included a short video clip as well as the camera calibration parameters. The camera calibration parameters must be known. 


**Requirements:**  
Python 3.8  
OpenCV  
Intrinsic camera parameters must be known for your camera.  

**Functionality:**  
To see the demo on provided video clip, simply call as:
```
python run_qr.py
```

If you want to use a webcam, call the function with the camera id. For example, webcam registered to 0: 
```
python run_qr.py 0
```

It is recommended that you keep your image resolution low (480p). If you want to use high resolution, resize the image to low resolution right before ```qr.detect()``` call and then rescale back to your full resolution.

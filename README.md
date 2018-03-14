# Advanced_Lane_Line_Detection

## Environment 
-Python                 
-OpenCV                     
-Numpy                    
-Matplotlib

## Steps
1. Compute the camera calibration matrix and distortion coefficients given a set of chessboard images.    
![Image text](https://github.com/Yunying-Chen/Advanced_Lane_Line_Detection/blob/master/img/undistort.jpg)                    
2. Apply a distortion correction to raw images.                                                         
3. Use Sobel X kernel, R channel and V channel to create a thresholded binary image.                         
![Image text](https://github.com/Yunying-Chen/Advanced_Lane_Line_Detection/blob/master/img/binary.jpg)                   
4. Apply a perspective transform to rectify binary image ("birds-eye view").                         
![Image text](https://github.com/Yunying-Chen/Advanced_Lane_Line_Detection/blob/master/img/straightLine.jpg)                 
![Image text](https://github.com/Yunying-Chen/Advanced_Lane_Line_Detection/blob/master/img/CurveLine.jpg)                 
5. Detect lane pixels and fit to find the lane boundary with sliding windows.  
![Image text](https://github.com/Yunying-Chen/Advanced_Lane_Line_Detection/blob/master/img/SlidingWindow.jpg)  
6. Determine the curvature of the lane and vehicle position with respect to center.                                              
7. Warp the detected lane boundaries back onto the original image.                           
8. Output visual display of the lane boundaries and numerical estimation of lane curvature and vehicle position.                       
![Image text](https://github.com/Yunying-Chen/Advanced_Lane_Line_Detection/blob/master/img/FillLane.jpg) 

## Performance
![GIF](https://github.com/Yunying-Chen/Advanced_Lane_Line_Detection/blob/master/img/Animation.gif)

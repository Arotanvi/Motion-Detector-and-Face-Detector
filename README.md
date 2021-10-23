# Motion-Detector-and-Face-Detector

"For Motion Detector"

Problem statement is - To show a dataframe using pandas which shows time intervals in which motion of a object was there and been captured by Computer's camera and at what time interval there was no motion . 

Library used - opencv , Pandas ,time

Steps Being followed-:-
1. To use videoCapture() method
2. to convert the frame to a gray image
3. to convert the frame to a gaussian image for increasing the efficiency of the gray image
4. to calculate the threshold and dilate the foreground object
5. Once dilation is done , capture the contours
6. to make a rectangle with help of contours
7. to show all this in specific windows and use key 'q' to destroy the windows and to stop computer from capturing the video
(=> 1 window will show gaussian video , 1 window will show normal colored video with a rectangle around it , 1 window will show threshold based video)

=>In order to show time intervals , make a list 'times' and append status into it and convert the list 'times' into required dataframe

=> Image data used to make a rectangle is a numpy matrix as python outputs the images while reading to a numpy matrix only

----------------------------------------------------------------------------------------------------------------------------------------------------

"For Face Detector"

Problem Statement - to detect the face from a image and to show a rectngle around facial part of image

Library used - opencv

Steps being followed:-

1.	To use cascade classifier to store the features/info of a face
2.	To read the image using cv2.imread() method
3.	To convert the image into gray image via cv2.cvtColor method
4.	Detect the face from gray image via detectMultiScale method
5.	to make a rectangle around the face of image
6.	resize the image obtained in step 5
7.	show it in a window using imshow() method and use destroyAllWindows() to close that window.


=> Image data obtained from detectMultiScale method is a numpy matrix 



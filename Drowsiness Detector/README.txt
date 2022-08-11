This project is made using DLIB, OpenCV and python.
The workflow of the Computer Vision Model is simple . 
The model is depended mainly on two variables :- 
1.The Detection of face from video stream, and landmark(in this project ,eyes) from live input video stream .
I have used the DLIB library for this purpose as it is as a really cool library for facial landmark detection.
2.Using the Euclidean Function to determine the eye ratio which  governs whether the eye is closed or open.
Ready for the core of this WHOLE PROJECT?
-The eye aspect ratio dynamically changes with each Video frame , and we have defined a threshold value beforehand.
When the ratio goes below the threshold value ,we start counting the number of frames for which the the value is below the threshold.
Why do we do this?Why don't we sound the alarm right away?
BECAUSE WE BLINK! So we have to make sure that the subject is not , we define a period of time(i.e,frames) for which the it is permissible for a person to BLINK.
When the frames increase a specified threshold value,WE GO AHEAD AND SOUND THE ALARM.

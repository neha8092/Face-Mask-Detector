
##  FACE MASK DETECTOR 

### Objective of this application is to detect people in an image or a video, and classify them into two classes Good and Bad based on whether they are wearing masks or not.



#### Below are the steps for inferencing the model on a video:-

1) Clone this repository in your system.
2) Once cloned , download the two files from the link mentioned - https://drive.google.com/drive/folders/1Vm8Tn9CktO5mCJwkC5NOG6g4Qt9O-CGh?usp=sharing  . These two files cannot be put into the github repo because of their size.
3) Place  'yolo-obj_best.weights' in the darknet/backup/ folder
4) Place 'yolo4.conv.137' in the darknet/build/darknet/x64/ folder
5) Run the python file - darknet_video.py for testing on videos. Below is the example to run the script.
 -- python darknet_video.py --location /data/test_video.mp4
 For the 'location' argument , provide the absolute path of the input video
 
 -- Result will be stored in the darknet folder with the name "Output.avi"
 
 
#### Below are the steps for inferencing the model on a image:-
Run the below command on the command line for images to be tested:

./darknet detector test ./build/darknet/x64/data/obj.data cfg/yolo-obj.cfg ./backup/yolo-obj_best.weights -ext_output /data/logo_detection/hack/test/test1.jpg

For the -ext_output argument, provide the absolute path od the input image


# Machine-Learning

Object Detection using YOLOv5 

This project is an application of object detection using YOLOv5, a deep-learning model for real-time object detection.
This project aims to detect the number plate of the cars in images or videos. 

Dataset 

The dataset used for this project is the custom dataset, which contains 50 images of cars with annotated number plates. The dataset is split into train and validation sets, with 80% and 20% of the images respectively. The dataset was annotated using the [MakeSense website], a free online tool for labeling images for computer vision applications. 

Model 

The model used for this project is YOLOv5s, the smallest and fastest variant of YOLOv5.
The model is trained on a custom configuration file that specifies the number of classes (1), the anchor boxes, and the hyperparameters.
The model is trained for 75 epochs using the Adam optimizer and a batch size of 16.
The model was trained on [Google Colab], which is a free cloud service that provides access to GPUs and TPUs. 

Counting Yellow Plates 

This project also includes a script that counts the number of yellow plates in the validation dataset. Yellow plates are used for commercial vehicles, and they can be distinguished from white plates by their color. The script uses OpenCV to convert the images to HSV color space and apply a mask to filter out the yellow pixels. If the percentage is greater than 50%, then the number plate is counted as yellow. 

Results 

The model achieves an average precision (AP) of 0.736 and an average recall (AR) of 0.774  on the validation set.
The model can detect most of the number plates of the cars in various lighting conditions, angles, and distances. 
Finally, the Number of yellow numberplates is detected and their count is given  

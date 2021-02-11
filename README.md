# Cigarette Smoking Detection using Deep Learning

This is a project of detecting Cigarette Smoking from the given images. The codes are based on implementation of Yolo-v3 by (https://github.com/AlexeyAB/darknet) on Python 3. The model generates bounding boxes for each instance of an object(Cigarette) in the image.

The codes and examples can be found in [smoking_detection.ipynb](smoking_detection.ipynb).

# Data

* I collect 659 smoking images from google images.
* I annotate all the images using [Yolo_mark](https://github.com/AlexeyAB/Yolo_mark).
* I split the images in 80% training images and 20% validation images.

# Training

* I use the Yolo-v3 by [https://github.com/AlexeyAB/darknet](https://github.com/AlexeyAB/darknet).
* I train the Yolo-v3 with pre-trained weights from [https://pjreddie.com/media/files/darknet53.conv.74](https://pjreddie.com/media/files/darknet53.conv.74) on Google Colab's Tesla K80 GPU for 1880 epochs.
* I got descent performance on the images and videos that were never been used in training.

You can find the training steps in [smoking_detection.ipynb](smoking_detection.ipynb).

# Result

<p float="left">
  <img src="smoking.jpg" width="415" height=315"/>
  <img src="smoking_det.jpg" width="415" height=315" /> 
</p>
<p float="left">
  <img src="smoking5.jpg" width="415" height=315"/>
  <img src="smoking5_det.jpg" width="415" height=315" /> 
</p>

You can also check the performance on this video [Smoking_detection.mp4](Smoking_detection.mp4).

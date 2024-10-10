# **Real-Time Object Detection using OpenCV and DNN**

This project demonstrates a simple implementation of real-time object detection using OpenCV's DNN module. It utilizes a pre-trained SSD MobileNet v3 model for object detection from live webcam feed. The detections are optimized by applying Non-Maximum Suppression (NMS) to filter out overlapping bounding boxes.

## **Features**
Real-time Object Detection: Detects objects in real-time using your webcam.
SSD MobileNet v3: A fast and lightweight object detection model.
Non-Maximum Suppression (NMS): Eliminates redundant bounding boxes to ensure accurate detections.
COCO Dataset Classes: Detects objects from the COCO dataset (80 classes).

## **Requirements**
Python 3.x
OpenCV 4.x
NumPy

## ** 1-Installation** 
Clone the repository: 

git clone https://github.com/yourusername/repo-name.git
cd repo-name

## ** 2-Install the required libraries: **

pip install opencv-python numpy

## ** 3-Download the necessary files: **

Pre-trained model weights: frozen_inference_graph.pb
Model configuration: ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt
COCO class names: coco.names

## **Code Overview **

-Model Setup: The pre-trained SSD MobileNet v3 model is loaded using OpenCV's DNN module. The input image is resized, scaled, and normalized for better detection accuracy.
-Object Detection: Object detection is performed on each frame captured from the webcam. The confidence score for each detected object is compared against a threshold to filter out weak detections.

-Non-Maximum Suppression (NMS): NMS is applied to remove overlapping bounding boxes, ensuring that only the most accurate detection for each object is shown.
-Bounding Boxes and Labels: Detected objects are highlighted with bounding boxes and labeled with the class name and confidence score.

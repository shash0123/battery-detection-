# battery-detection-

Model Overview
We have utilized multiple YOLO (You Only Look Once) models for object detection tasks, including
YOLOv3, YOLOv7 and YOLOv8. These models are known for their efficiency and high accuracy
in detecting objects in images.

Performance Metrics and Accuracy

a. YOLOv3
 Parameters: IoU Loss (mse), IoU Norm (0.75), Obj Norm (1.00), Delta Norm (1.00).
 Accuracy: 92.40% (mAP@0.50).
 Class-wise Accuracy:
o 9V: 91.85%
o Coincell: 90.52%
o Drycell: 94.83%
 Inference Time: 1 second.
 Additional Notes: Precision = 0.81, Recall = 0.88, F1-score = 0.85.

c. YOLOv7
 Parameters: 168 layers, trained for 100 epochs.
 Accuracy: 99.5% (mAP@0.50).
 Class-wise Accuracy:
o 9V: 99.5%
o Coincell: 99.6%
o Drycell: 99.5%
 Inference Speed: ~8-12 ms per image

d. YOLOv8
 Parameters: 168 layers, 11,126,745 parameters, 28.4 GFLOPs.
 Accuracy: 99.2% (mAP@0.50).
 Class-wise Accuracy:
o 9V: 98.7%
o Coincell: 99.5%
o Drycell: 99.3%
 Inference Speed: ~2.4 images/second.

Hardware Used
All models were trained and tested on my laptop with the following specifications:
 GPU: NVIDIA T4 GPU (15 GB RAM)
 RAM: 12.7 GB
 Processor: Intel Xeon processors.
 Storage: 112.7 GB

Data Collection
The dataset used is open source, containing images of batteries (9V, coincell, drycell) along with their
labels. This allows for transparent reproducibility and benchmarking.

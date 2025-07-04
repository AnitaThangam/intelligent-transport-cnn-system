# Intelligent-transport-cnn-system
A CNN-powered solution for real-time traffic detection, vehicle classification, and estimating traffic volume to support smart transportation systems.

**Project Architecture**

![image](https://github.com/user-attachments/assets/2c5d640f-2526-4071-a2ee-82d40cafd62e)

**Freatures**

**Traffic Object Detection**
Detects vehicles in images or video streams using CNN-based models (e.g., YOLO, SSD, Faster R-CNN).

Real-time or batch processing supported.

**Vehicle Classification**
Classifies detected vehicles into categories like car, bus, truck, and motorcycle.

Leverages transfer learning with pretrained models (e.g., ResNet, VGG).

**Traffic Volume Estimation**
Counts vehicles across predefined zones or lines over time.

Supports both frame-wise and region-based volume aggregation.

**Input Support**-
Accepts real-time traffic camera feeds or pre-recorded video files.

Supports image sequences and single-frame inference.

**Data Preprocessing**
Image normalization, resizing, and augmentation (e.g., flipping, cropping).

Support for COCO, Pascal VOC, or custom annotation formats.

**Model Framework**
Built using PyTorch (or TensorFlow) for training and inference.

Exportable to ONNX or TorchScript for deployment.

**Evaluation Metrics**
Object detection: mAP (mean Average Precision)

Classification: Accuracy, Precision, Recall, F1-score

Volume estimation: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE)

**Post-Processing**
Non-Maximum Suppression (NMS) to refine detection outputs.

Optional object tracking using SORT or Deep SORT for accurate volume counting.

**Dataset Information**

File:
traffic_dataset_large.csv

Fields:
image_id: Identifier of the image or frame
vehicle_type: Category label (e.g., car, truck, bus, motorcycle)
bounding_box: Coordinates for object detection (x_min, y_min, x_max, y_max)
frame_time: Timestamp for each frame (optional for volume estimation)
count: Number of vehicles in the frame or region (for volume estimation)

Annotations:
Vehicle detection and classification are labeled for each frame
Ground truth counts provided for evaluating traffic volume estimation
Format compatible with most deep learning frameworks (e.g., COCO-style or custom parsers)

**Accuracy:**
Classification (Vehicle Type):
Accuracy: 91.3%

Precision: 90.8%

Recall: 89.7%

F1 Score: 90.2%

**Metrics:**
Volume Estimation (Vehicle Counting):
Mean Absolute Error (MAE): 2.3 vehicles per frame

Root Mean Squared Error (RMSE): 3.1 vehicles

**Result**
Counting Accuracy: 92.5%

**Citation:**

  title     = {A CNN-Based Framework for Accurate Traffic Detection, Classification, and Volume Estimation in Intelligent Transportation Systems},
  author    = {Anita Thangam C and Kavitha T},
  booktitle = {Proceedings of the International Conference on Computing, Communication and Artificial Intelligence (ICCCAI 2025)},
  year      = {2025},
  publisher = {Springer},
  note      = {Accepted for publication},
  address   = {Karunya Institute of Technology and Sciences, Coimbatore, India}





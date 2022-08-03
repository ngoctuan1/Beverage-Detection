1. Training: yolov7_training.ipynb
- Download Dataset from Robotflow: Đã download trong folder drinks-1
- Install Enviroment: Pytorch + requirements.txt
- Detect

2. Guide: Chạy file clients.py
- Leak mem -> comment dòng x[:, 5:] *= x[:, 4:5]  # conf = obj_conf * cls_conf trong file ultis/general.py (dòng 648->652)

3. Điều chỉnh tham số truyền vào class coke trong file client.py

param weights: the path to the weights file
param source: the path to the video file
param conf: the confidence threshold for the bounding boxes
param imgsz: The size of the image to be processed, defaults to 640 (optional)
param device: the GPU device to use, defaults to 0 (optional)
param iou_thres: The IoU threshold for non-maximum suppression

4. Ảnh sau khi Detect sẽ được lưu trong run/detect/exp
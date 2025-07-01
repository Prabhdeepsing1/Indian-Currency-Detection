# YOLO Custom Object Detection Model

This repository contains a custom-trained YOLO object detection model using the [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) framework. The model (`my_model.pt`) was trained on a custom dataset using Google Colab and is ready for use in real-world object detection tasks.

---

## 📁 Repository Structure
. .

├──my_model.pt # Trained YOLO model (custom)

├── yolo_detect.py # Inference script

├── requirements.txt # Python dependencies

├── README.md # Project documentation

├── Results # Folder containing result of test images

├── Weights # Folder containing Weights of the model post training

---

## 🚀 Installation

1. **Clone the repository**
```bash
git clone https://github.com/your-username/yolo-custom-model.git
cd yolo-custom-model
```
2. **Create and activate a virtual environment (optional but recommended)**

```bash
python -m venv venv
source venv\Scripts\activate
```
3. **Install dependencies**
```bash
pip install -r requirements.txt
```

## 🎯 Run Inference
Use the command below to detect objects on images, videos, or webcam:
```bash
python yolo_detect.py --model my_model.pt --source <path/to/image-or-video-or-0>
```

Examples
#### Detect on an image:

```bash
python yolo_detect.py --model my_model.pt --source images/sample.jpg
```
#### Detect on a folder:
```bash
python yolo_detect.py --model my_model.pt --source images/
```
#### Detect using webcam:
```bash
python yolo_detect.py --model my_model.pt --source 0
```

## 🧠 Model Info
Model Format: PyTorch (.pt)

Framework: Ultralytics YOLO

Training Platform: Google Colab

Dataset: Custom (user-defined)



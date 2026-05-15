# Real-Time Object Detection using TensorFlow and OpenCV

A real-time object detection system built using TensorFlow, OpenCV, and the SSD MobileNet V2 model.

The application detects objects from a webcam feed and displays:
- Bounding boxes
- Object labels
- Confidence scores
- Real-time FPS counter

---

# Features

- Real-time webcam object detection
- TensorFlow SSD MobileNet model
- OpenCV visualization
- FPS monitoring
- Frame skipping optimization
- Screenshot capture support
- Lightweight and optimized for CPU usage

---

# Technologies Used

- Python
- TensorFlow
- OpenCV
- NumPy

---

# Model Used

Model:
`ssd_mobilenet_v2_fpnlite_640x640_coco17_tpu-8`

Dataset:
COCO Dataset (90 classes)

Framework:
TensorFlow Object Detection API

---

# Project Structure

```text
ObjectDetectionProject/
│
├── Model/
│   └── ssd_mobilenet_v2_fpnlite_640x640_coco17_tpu-8/
│       └── saved_model/
│
├── main.py
├── requirements.txt
└── README.md
```

---

# Installation

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/object-detection-project.git
cd object-detection-project
```

---

## 2. Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / Mac

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install tensorflow opencv-python numpy
```

---

# Download TensorFlow Model

Download the model from TensorFlow Model Zoo.

Model Link:
https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/training.html

After downloading, place the model folder inside:

```text
Model/
```

Final path should look like:

```text
Model/ssd_mobilenet_v2_fpnlite_640x640_coco17_tpu-8/saved_model
```

---

# Running the Project

Run the Python file:

```bash
python main.py
```

---

# Controls

| Key | Action |
|-----|--------|
| Q | Quit Application |
| S | Save Screenshot |

---

# Optimizations Used

- Reduced webcam resolution
- Frame skipping
- FPS smoothing
- Reusing previous detections
- Small input frame processing

---

# Output

The application displays:

- Real-time object detection
- Bounding boxes
- Class names
- Detection confidence
- FPS counter

---

# Example Classes Detected

- Person
- Car
- Dog
- Cat
- Laptop
- Cell Phone
- Bottle
- Chair
- TV

and many more...

---

# Future Improvements

- GPU acceleration
- Multi-threading
- YOLO integration
- TensorRT optimization
- ONNX conversion
- Custom object training

---

# Requirements

Example `requirements.txt`

```text
tensorflow
opencv-python
numpy
```

---

# Troubleshooting

## No module named cv2

Install OpenCV:

```bash
pip install opencv-python
```

---

## TensorFlow not found

Install TensorFlow:

```bash
pip install tensorflow
```

---

## SavedModel file does not exist

Check the model path:

```python
path_to_model = r"Model/ssd_mobilenet_v2_fpnlite_640x640_coco17_tpu-8/saved_model"
```

Ensure:
- `saved_model.pb` exists
- `variables` folder exists

---

# Performance Tips

For better FPS:

- Use `320x320` model
- Reduce webcam resolution
- Use GPU acceleration
- Run detection every few frames

---

# License

This project is open-source and available under the MIT License.

---

# Author

Developed using:
- TensorFlow
- OpenCV
- Python
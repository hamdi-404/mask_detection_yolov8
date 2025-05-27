# Real-Time Face Mask Detection Using YOLOv8 😷🎯

This project detects whether a person is:
- Wearing a mask correctly 😷
- Wearing a mask incorrectly 😕
- Not wearing a mask at all 😐

The detection runs in **real-time using your webcam** and is powered by **YOLOv8** from Ultralytics.

## 📁 Project Structure

```
mask_detection_yolov8/
├── best.pt                   # Trained YOLOv8 model weights
├── detect_webcam.py          # Script to run real-time webcam detection
├── notebooks/
│   └── train_and_demo.ipynb  # Notebook for training & testing
├── requirements.txt          # List of dependencies
└── README.md                 # Project documentation
```

## 📦 Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

## 🧪 How to Run

1. Make sure your webcam is connected.
2. Run the real-time detection:

```bash
python detect_webcam.py
```

## 📊 Training Summary

- **Model**: YOLOv8 (Ultralytics)
- **Classes**:
  - `with_mask`
  - `without_mask`
  - `incorrect_mask`
- **Dataset**: Custom-labeled dataset in YOLO format
- **Training**: Fine-tuned with augmentation & validation monitoring
- **Performance**: Trained model saved as `best.pt`

## 🎥 Demo

👉 [Click to watch demo](./video_demo_1.mp4)

## ✨ Credits

- [YOLOv8 by Ultralytics](https://github.com/ultralytics/ultralytics)
- OpenCV for webcam integration
- Custom dataset annotations

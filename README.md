# Cheating Hand Sign Detector with YOLOv8 🚨✋

This project fine-tunes a YOLOv8 model to detect anomalous hand gestures (potential cheating signs) in examination footage.

## 🔍 Overview
- Model: `YOLOv8m`
- Dataset: Custom-annotated Roboflow dataset (1 class: `CheatingHandSign`)
- Trained on: RTX 2070 GPU
- Use case: Detect cheating hand gestures in classroom surveillance videos.

## 📊 Performance (Final Metrics)
| Metric           | Value     |
|------------------|-----------|
| Precision        | 0.92      |
| Recall           | 0.91      |
| mAP@0.5          | 0.97      |
| mAP@0.5:0.95     | 0.71      |

## 🧠 Sample Results
| Detection Frame | Description |
|------------------|-------------|
| ![](results/predictions/sample1.jpg) | Correctly detected hand signal |
| ![](results/predictions/sample2.jpg) | Missed normal hand gesture |

## 🏗️ Project Structure
- `data/` – Training and validation sets
- `notebooks/train_yolov8m.ipynb` – Training notebook
- `weights/best.pt` – Final trained model
- `videos/output_annotated.mp4` – Model inference on sample video

## 🛠️ How to Run
1. Clone the repo:
```bash
git clone https://github.com/yourusername/cheating-handsign-detector-yolov8.git
cd cheating-handsign-detector-yolov8

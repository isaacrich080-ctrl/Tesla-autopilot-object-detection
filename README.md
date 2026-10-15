# Tesla-autopilot-object-detection
Tesla Autopilot Clone using YOLO for road object detection with the KITTI dataset.
# 🚗 Tesla Autopilot Clone – Object Detection

## 📌 Project Overview

The **Tesla Autopilot Clone – Object Detection** project demonstrates the use of computer vision and deep learning to identify and locate objects in road-scene images. Inspired by autonomous driving technology, this project uses the KITTI dataset and the YOLO object detection framework to detect road users and vehicles.

The system aims to identify objects such as cars, pedestrians, cyclists, trucks, vans, and other supported categories using bounding boxes.

**Note:** This is an educational prototype and is not intended for real-world autonomous vehicle control.

## 🎯 Objectives

- Understand the fundamentals of object detection and computer vision.
- Explore and preprocess the KITTI road-scene dataset.
- Convert KITTI annotations into YOLO-compatible format.
- Prepare images and labels for model training.
- Train and evaluate a YOLO object detection model.
- Visualize detected objects with bounding boxes and confidence scores.
- Explore the applications of object detection in autonomous driving.

## 🛠️ Technologies Used

- Python
- YOLO (Ultralytics)
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Pillow (PIL)
- Jupyter Notebook
- Kaggle Notebook
- KITTI Dataset

## 📊 Dataset Description

This project uses the **KITTI Vision Benchmark Suite**, which provides images and annotations for computer vision research in autonomous driving.

The dataset contains road-scene images and object annotations, including bounding-box coordinates.

### Object Classes

The project maps the following KITTI categories to class IDs:

| Class ID | Object Class |
|---:|---|
| 0 | Car |
| 1 | Van |
| 2 | Truck |
| 3 | Pedestrian |
| 4 | Person Sitting |
| 5 | Cyclist |
| 6 | Tram |
| 7 | Miscellaneous |

Annotations belonging to the `DontCare` category are excluded during preprocessing.

Dataset source: https://www.cvlibs.net/datasets/kitti/

## ⚙️ Project Methodology

### 1. Importing Libraries
Import the required Python libraries for data processing, image handling, visualization, and object detection.

### 2. Dataset Loading
Locate the KITTI training images and their corresponding annotation files.

### 3. Data Preprocessing
Read the original annotation files and extract object classes and bounding-box coordinates.

### 4. Label Conversion
Convert the original KITTI bounding boxes into YOLO format:

`class_id x_center y_center width height`

Bounding-box coordinates are normalized relative to image width and height.

### 5. Dataset Preparation
Organize the images and labels into the required directory structure and prepare the dataset configuration for YOLO.

### 6. Model Training
Configure the YOLO model and train it using the prepared dataset.

### 7. Model Evaluation
Evaluate the trained model using suitable object detection metrics, such as precision, recall, and mean Average Precision (mAP).

### 8. Object Detection and Visualization
Run inference on test images and display the predicted object classes, bounding boxes, and confidence scores.

## 📂 Project Structure

```text
tesla-autopilot-object-detection/
│
├── Tesla_Autopilot_Object_Detection.ipynb
├── README.md
├── data.yaml
├── images/
│   ├── train/
│   └── val/
└── labels/
    ├── train/
    └── val/
```

*Note: The directory structure above is an example. Update it to match the actual files in your repository.*

## 💻 Installation

Install the required libraries:

```bash
pip install ultralytics numpy pandas matplotlib scikit-learn tqdm pillow opencv-python
```

## ▶️ How to Run

1. Open the notebook in Kaggle or Jupyter Notebook.
2. Configure the dataset path according to your environment.
3. Run the notebook cells in sequence.
4. Complete dataset preprocessing and label conversion.
5. Configure and train the YOLO model.
6. Evaluate the model and visualize the detection results.

## 📈 Results and Evaluation

The project is designed to demonstrate road-object detection using YOLO.

Evaluation can include:

- **Precision:** Measures how many predicted objects are correct.
- **Recall:** Measures how many actual objects are detected.
- **mAP@50:** Evaluates detection accuracy at an IoU threshold of 0.50.
- **mAP@50–95:** Evaluates performance across multiple IoU thresholds.
- **Inference time:** Measures the time required to process an image.

Add your actual training metrics, output screenshots, and observations here after running the model. Do not report unmeasured results.

## ⚠️ Limitations

- Detection performance depends on dataset quality and training.
- Small, distant, or partially hidden objects may be difficult to detect.
- Performance may vary with lighting, weather, and road conditions.
- This prototype is not validated for real-world vehicle control.

## 🔮 Future Enhancements

- Extend object detection to video streams.
- Explore real-time detection using a webcam.
- Improve detection of small and distant objects.
- Compare different YOLO model versions.
- Optimize inference speed and detection accuracy.
- Explore integration with lane detection and road-scene analysis.

## 📝 Conclusion

This project demonstrates a computer vision workflow for autonomous-driving-inspired object detection, including dataset preprocessing, annotation conversion, model training, evaluation, and visualization.

It provides practical experience with Python, deep learning, and object detection while illustrating how computer vision can contribute to intelligent transportation systems.

## 👨‍💻 Author

**Your Name**

GitHub: https://github.com/your-username


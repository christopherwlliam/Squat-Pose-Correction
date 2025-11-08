# 🧠 Application of YOLO–MediaPipe Based Deep Learning for Detection and Correction of Incorrect Squat Posture

This repository contains the implementation and supporting materials for the research titled  
**“Application of YOLO–MediaPipe Based Deep Learning for Detection and Correction of Incorrect Squat Posture.”**

The project focuses on developing an intelligent system that combines **pose estimation** and **ensemble learning** to automatically detect and classify squat posture accuracy.  
The system extracts body keypoints and computes biomechanical angles from side-view images using **MediaPipe** and **YOLOv8-Pose**, then classifies them into three posture categories:  
**Good**, **Bad Back**, and **Bad Heel**.

---

## ⚙️ Key Features
- Integration of **MediaPipe** and **YOLOv8** for human pose estimation.  
- Extraction of **biomechanical angles** (hip, knee, and back) for feature enhancement.  
- Implementation of **ensemble learning algorithms**: LightGBM, Random Forest, and Bagging.  
- Evaluation based on **accuracy, precision, recall, and F1-score** metrics.  
- Application of **SMOTE** for class balancing to improve fairness in training.

---

## 📊 Research Results
| Classifier | Accuracy | Notes |
|-------------|-----------|-------|
| **LightGBM** | 91.82% | Highest performance with MediaPipe keypoints |
| **Random Forest** | 90.78% | Strong generalization and stable results |
| **Bagging** | 86.46% | Better recall for minority (Bad Heel) class |

---

## 📂 Repository Structure
```
/code/ → Model training, preprocessing, and pose estimation scripts
/dataset/ → Dataset description and download link
/README.md → Project overview (this file)
```

---

## 📦 Dataset
The dataset used in this study is publicly available on **Zenodo**:  
📘 **DOI:** [10.5281/zenodo.17558629](https://doi.org/10.5281/zenodo.17558629)

It contains side-view squat images labeled as *Good*, *Bad Back*, and *Bad Heel*,  
formatted in a 1:1 aspect ratio for pose estimation experiments.

---

## 🧠 Citation
> Christopher William. (2025). *Application of YOLO–MediaPipe Based Deep Learning for Detection and Correction of Incorrect Squat Posture.*

Dataset: [https://doi.org/10.5281/zenodo.17558629](https://doi.org/10.5281/zenodo.17558629)

---

## 🤝 Contact
For questions, collaboration, or feedback, please contact:  
📧 **christopher.teng@binus.ac.id**


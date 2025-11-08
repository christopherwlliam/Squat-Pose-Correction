# 🧠 Squat Posture Classification Dataset

📘 **DOI:** [10.5281/zenodo.17558629](https://doi.org/10.5281/zenodo.17558629)  
📅 **Version:** 1.0  
📂 **Resource Type:** Dataset  
👤 **Author:** Christopher William  

---

## 📖 Overview
This dataset was developed to support research on **Application of YOLO–MediaPipe Based Deep Learning for Detection and Correction of Incorrect Squat Posture**.  
It contains **side-view images** of individuals performing squats categorized into three classes:
- 🟩 **Good** – Correct squat posture  
- 🟥 **Bad Back** – Incorrect spinal alignment  
- 🟨 **Bad Heel** – Heel elevation or foot instability  

Each image is formatted in a **1:1 aspect ratio** to maintain consistency during preprocessing and pose estimation.

The dataset was used in research comparing **MediaPipe** and **YOLOv8-Pose** for keypoint extraction, and in evaluating ensemble classifiers such as **LightGBM**, **Random Forest**, and **Bagging** for accurate squat posture classification.

---

## 🧩 Dataset Structure
```
Dataset/
│
├── train/
│ ├── Good/
│ │ ├── Good_001.jpg
│ │ ├── Good_002.jpg
│ │ └── ...
│ │
│ ├── Bad_Back/
│ │ ├── Bad_Back_001.jpg
│ │ ├── Bad_Back_002.jpg
│ │ └── ...
│ │
│ └── Bad_Heel/
│ ├── Bad_Heel_001.jpg
│ ├── Bad_Heel_002.jpg
│ └── ...
│
└── test/
├── Good/
│ ├── Good_001.jpg
│ ├── Good_002.jpg
│ └── ...
│
├── Bad_Back/
│ ├── Bad_Back_001.jpg
│ ├── Bad_Back_002.jpg
│ └── ...
│
└── Bad_Heel/
├── Bad_Heel_001.jpg
├── Bad_Heel_002.jpg
└── ...
```

Each folder represents a **posture category**, with side-view squat images saved in `.jpg` format.

---

## ⚙️ Technical Details
- **Image Format:** JPG  
- **Aspect Ratio:** 1:1  
- **Viewpoint:** Side-view  
- **Pose Estimation Frameworks:** MediaPipe, YOLOv8-Pose  
- **Classifiers Evaluated:** LightGBM, Random Forest, Bagging  
- **Preprocessing:** Data normalization, augmentation (flip, rotation, brightness, contrast), and SMOTE balancing for minority classes  

---

## 🧪 Research Context
The dataset was used in the study *“Deep Learning–Based Squat Posture Classification using MediaPipe and YOLOv8”*, focusing on biomechanical feature extraction and ensemble learning for fitness posture analysis.  
Experimental results showed that:
- **LightGBM** achieved the highest accuracy (**91.82%**) using MediaPipe keypoints.  
- **Random Forest** provided strong generalization with balanced precision and recall.  
- **Bagging** offered higher recall for minority classes, particularly for *Bad Heel* detection.  

---

## 🧑‍💻 Recommended Use
This dataset is suitable for:
- Pose estimation and human keypoint detection  
- Exercise posture classification research  
- Real-time movement correction systems  
- Fitness technology and sports analytics  

---

## ⚖️ License and Citation
This dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.  
You are free to use, share, and adapt the dataset with appropriate credit to the author.

### **Citation**
> Christopher William. (2025). *Application of YOLO–MediaPipe Based Deep Learning for Detection and Correction of Incorrect Squat Posture* [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.17558629](https://doi.org/10.5281/zenodo.17558629)

---

## 🤝 Contributions and Contact
Contributions, feedback, or collaboration inquiries are welcome.  
For questions, please contact:  
📧 **christopher.teng@binus.ac.id**

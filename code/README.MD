# Application of YOLO–MediaPipe Based Deep Learning for Detection and Correction of Incorrect Squat Posture [CODE]

This repository provides a complete pipeline for **squat posture classification** using pose landmark extraction (MediaPipe & YOLOv8), angle computation, dataset balancing using SMOTE, and machine learning classification.

The project is optimized for **Google Colab** and uses Google Drive for dataset handling.

---

## 🚀 Features

### **1. Data Preprocessing**
- Image resizing (640×640)
- Data augmentation using **Albumentations**:
  - Horizontal flip  
  - Brightness/contrast  
  - Rotation ±15°  
  - Motion blur  
- Output saved to: `Dataset_Augmented/`

---

### **2. Landmark Extraction**
#### **MediaPipe Pose (33 Keypoints)**
Output files:
- `mediapipe_train_landmarks.xlsx`
- `mediapipe_test_landmarks.xlsx`

#### **YOLOv8 Pose (17 Keypoints)**
Output files:
- `yolo_train_landmarks.xlsx`
- `yolo_test_landmarks.xlsx`

---

### **3. Angle Calculation**
Angles extracted from landmark coordinates:
- Left/Right Knee  
- Left/Right Hip  
- Left/Right Shoulder  

Results:
- `mediapipe_train_angles.xlsx`
- `mediapipe_test_angles.xlsx`
- `yolo_train_angles.xlsx`
- `yolo_test_angles.xlsx`

---

### **4. Dataset Balancing (SMOTE)**
SMOTE applied to:
- Landmark files  
- Angle files  

Outputs:
- Override mode  

---

### **5. Machine Learning Models**
Implemented:
- **Random Forest**
- **LightGBM**
- **Bagging (Decision Tree)**

Used on:
- MediaPipe Landmarks  
- MediaPipe Angles  
- YOLO Landmarks  
- YOLO Angles  

---

## 📁 Folder Structure
```
/content/drive/MyDrive/
├── Dataset/ # raw images
├── Dataset_Augmented/ # augmented output
├── Dataset_Excel/ # Excel results
```

## 📁 Google Drive ensures:

- ✔ Persistent storage (Colab resets won't delete files)  
- ✔ Large dataset handling  
- ✔ Simple file management  
- ✔ Organized workflow  

Before running any script, mount Google Drive:

```
from google.colab import drive
drive.mount('/content/drive')
```


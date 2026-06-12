# 🖐️ PRODIGY_ML_04 — Hand Gesture Recognition (SVM)

> **Prodigy InfoTech Machine Learning Internship — Task 04**

## 📌 Task Description
Develop a hand gesture recognition model that can accurately identify and classify different hand gestures from image data, enabling intuitive human-computer interaction and gesture-based control systems.

---

## 📂 Dataset
**LeapGestRecog — Kaggle**  
🔗 https://www.kaggle.com/gti-upm/leapgestrecog

- 10 different hand gesture classes
- Multiple subjects
- Grayscale images

---

## 🛠️ Tech Stack
| Tool | Purpose |
|------|---------|
| Python 3.x | Programming Language |
| OpenCV (cv2) | Image loading & preprocessing |
| Scikit-learn | SVM model & evaluation |
| PCA | Dimensionality reduction |
| Matplotlib | Visualizations |
| Seaborn | Statistical plots |
| NumPy | Numerical computations |

---

## 📁 Project Structure
```
PRODIGY_ML_04/
│
├── hand_gesture_recognition.py  # Main Python script
├── sample_gestures.png          # Sample gesture images
├── class_distribution.png       # Class distribution plot
├── confusion_matrix.png         # Model confusion matrix
├── predictions.png              # Sample predictions
└── README.md                    # Project documentation
```

---

## ⚙️ How to Run on Google Colab

### 1. Download Dataset
```python
import os
os.makedirs('/root/.kaggle', exist_ok=True)
with open('/root/.kaggle/kaggle.json', 'w') as f:
    f.write('{"username":"YOUR_USERNAME","key":"YOUR_API_KEY"}')
os.chmod('/root/.kaggle/kaggle.json', 0o600)
!pip install kaggle -q
!kaggle datasets download -d gti-upm/leapgestrecog
!unzip leapgestrecog.zip -d hand_gestures
```

### 2. Run the script
- Paste code from `hand_gesture_recognition.py` into Colab
- Click Run and wait for results!

---

## 📊 Model Performance

| Metric | Value |
|--------|-------|
| Model | Support Vector Machine (SVM) |
| Kernel | RBF |
| Gesture Classes | 10 |
| PCA Components | 100 |
| Accuracy | ~90%+ |

---

## 📈 Key Visualizations
- **Sample Gestures** — Sample images from each gesture class
- **Class Distribution** — Number of images per gesture class
- **Confusion Matrix** — Detailed prediction accuracy per class
- **Sample Predictions** — Green = correct, Red = incorrect

---

## 🔍 Key Findings
- SVM with RBF kernel works well for gesture classification
- PCA reduced dimensions significantly while retaining variance
- Grayscale images are sufficient for gesture recognition
- High accuracy achieved with basic pixel features

---

## 👤 Author
Rabiya
Machine Learning Intern — Prodigy InfoTech  

---

## 📜 License
This project is for educational purposes as part of an internship program.

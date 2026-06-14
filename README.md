# 🖼️ CNN-Based Image Forgery Detection System

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Accuracy](https://img.shields.io/badge/Detection%20Accuracy-Improved%2015%25-brightgreen)
![Architecture](https://img.shields.io/badge/Architecture-Meso4%20CNN-purple)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Overview

A **deep learning-based Image Forgery Detection System** that identifies digitally manipulated images using the **Meso4 CNN architecture** with **TensorFlow**. The system detects face manipulation forgeries (deepfakes) in images with high precision, reducing false positives by **20%** over the baseline model.

Built with a clean **HTML5/CSS3 web interface** integrated with a **Python Flask backend** — users can upload images and receive instant forgery detection results with confidence scores.

---

## 🏆 Key Results

| Metric | Baseline | Our Model | Improvement |
|--------|----------|-----------|-------------|
| Detection Accuracy | — | +15% over baseline | ✅ |
| False Positive Rate | baseline | -20% reduction | ✅ |
| Test Samples | 1,000+ images | 1,000+ images | — |
| Architecture | Standard CNN | Meso4 (optimised) | ✅ |

- ✅ **15% accuracy improvement** over baseline through iterative model optimisation
- ✅ **20% reduction in false positives** through threshold tuning and data augmentation
- ✅ **1,000+ image samples** tested across multiple forgery categories
- ✅ **Responsive web interface** — upload image, get result instantly
- ✅ **Comprehensive documentation** — UI specs, flowcharts, test results

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Deep Learning | TensorFlow 2.x, Keras, Meso4 CNN Architecture |
| Backend | Python, Flask, REST API |
| Frontend | HTML5, CSS3, Bootstrap, JavaScript |
| Data Processing | NumPy, Pandas, OpenCV, Pillow |
| Database | SQL (image metadata storage) |
| Version Control | Git, GitHub |

---

## 🧠 How It Works

```
Input Image
     │
     ▼
Preprocessing (resize → 256x256, normalize pixel values)
     │
     ▼
Meso4 CNN Feature Extraction
(4 convolutional blocks → max pooling → batch normalisation)
     │
     ▼
Fully Connected Classifier
     │
     ▼
Output: REAL / FORGED + Confidence Score (0–100%)
```

**Meso4 Architecture** is specifically designed to detect mesoscopic properties of images — the subtle inconsistencies in texture and noise patterns introduced by digital manipulation tools — making it highly effective for deepfake and splicing detection.

---

## 📁 Project Structure

```
Image-Forgery-Detection-System/
│
├── app/
│   ├── app.py                  # Flask application
│   ├── templates/
│   │   └── index.html          # Upload interface (HTML5/CSS3)
│   └── static/
│       ├── css/style.css       # Responsive CSS
│       └── js/main.js          # JavaScript file upload handler
│
├── model/
│   ├── meso4_model.py          # Meso4 CNN architecture
│   ├── train.py                # Model training script
│   └── evaluate.py             # Evaluation & metrics
│
├── data/
│   ├── preprocess.py           # Image preprocessing pipeline
│   └── augment.py              # Data augmentation
│
├── notebooks/
│   └── Forgery_Detection.ipynb # Training notebook with results
│
├── docs/
│   ├── UI_Specifications.pdf   # UI flowcharts and specs
│   └── Test_Results.pdf        # Full test documentation
│
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Lokesh1509/Image-Forgery-Detection-System.git
cd Image-Forgery-Detection-System
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the Flask web app
```bash
python app/app.py
```

### 4. Open in browser
```
http://localhost:5000
```

### 5. Upload an image
- Click **"Choose Image"**
- Select any `.jpg`, `.png`, or `.jpeg` file
- Click **"Detect Forgery"**
- View result: **REAL** or **FORGED** with confidence score

---

## 📦 Requirements

```
flask==2.3.0
tensorflow==2.12.0
keras==2.12.0
numpy==1.24.0
pandas==2.0.0
opencv-python==4.7.0
Pillow==9.5.0
scikit-learn==1.2.2
matplotlib==3.7.1
```

---

## 🧪 Testing

The system was tested on **1,000+ image samples** across multiple forgery categories:

| Forgery Type | Description |
|-------------|-------------|
| Deepfake | AI-generated face manipulation |
| Splicing | Image regions combined from multiple sources |
| Copy-Move | Region duplicated within same image |
| Retouching | Localised pixel manipulation |

Test documentation including flowcharts, UI specifications, and full results available in `/docs/`.

---

## 📊 Training Details

- **Dataset:** Custom dataset + public forgery detection benchmarks
- **Architecture:** Meso4 CNN (4 convolutional blocks)
- **Optimiser:** Adam (lr=0.001)
- **Batch size:** 32
- **Epochs:** 50 with early stopping
- **Augmentation:** Horizontal flip, rotation, brightness adjustment

---

## 👤 Author

**Polagoni Lokesh**  
B.Tech — Computer Science & Engineering (Cyber Security)  
Anurag University, Hyderabad  
📧 polagonilokesh739@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/polagoni-lokesh) | [GitHub](https://github.com/Lokesh1509)

---

## 🔗 Related Project

Also check out my IEEE-published **Intrusion Detection System**:  
👉 [Deep-Learning-Intrusion-Detection-System](https://github.com/Lokesh1509/Deep-Learning-Intrusion-Detection-System)

---

## 📜 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

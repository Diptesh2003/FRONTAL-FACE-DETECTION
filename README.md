# 👁️ Frontal Face Detection ML OpenCV

## 🧐 Overview
This repository provides a complete, modular pipeline for real-time **frontal face detection** and recognition using **OpenCV** and **Machine Learning** (Keras). Stream images from a webcam/IP camera, preprocess faces, train a CNN, and perform accurate face recognition! Perfect for ML engineers, computer vision researchers, or hobbyists.

---

## ⚡️ Features
- 📦 **Data Acquisition**: Stream frames from an IP camera and auto-capture face samples using Haar Cascade.
- 🧹 **Preprocessing**: Convert images to grayscale, resize, histogram equalization.
- 🏷️ **Labeling & Serialization**: Automate labeling and storage using Pickle.
- 🧠 **Model Inference**: Use a trained deep neural network (Keras `.h5` model) for robust face recognition.
- 🎥 **Real-time Detection**: Instantaneous predictions on live video feeds.

---

## 🚀 Quick Start

### 1. 💾 Data Collection
Run `collect_data.py` to capture face images directly from your webcam/IP-cam:
- **Stores**: 100 face samples per subject in `Images/`.
- **Dependencies**: `opencv-python`, `numpy`, `urllib`.

### 2. 📊 Data Consolidation
Preprocess, resize, and serialize your images & labels:
- **Serialized Data**: Saved to `TESTING/images.p` and `TESTING/labels.p`.

### 3. 🧠 Model Training *(not included)*
Train your own CNN model (see documentation for recommended pipeline).

### 4. 🔍 Face Recognition
Connect your trained model & run live recognition:
- **Predicts facial identity in real-time!**

---

## 🛠️ Tech Stack
- **OpenCV**: Haar Cascade Classifier for face region proposal.
- **Keras/TensorFlow**: Deep neural network model for face classification.
- **NumPy, Pickle**: Efficient data wrangling and persistence.
- **matplotlib**: For quick image visualizations.

---

## 💡 Usage Tips
- Make sure your `haarcascade_frontalface_default.xml` and trained `final_model.h5` are in the specified paths.
- Tune detection parameters for your specific lighting and camera setup.
- Extend the label set in `recognize.py` as needed.

---

## 📁 Directory Structure

---

## 👨‍💻 Author
- 🧑‍💻 *Your Name* — ML & CV Enthusiast

---

## 📝 License
[MIT License](LICENSE)

---

## 🌟 Contributing
PRs and Issues welcome! Please ensure your code adheres to the repo’s style.

---

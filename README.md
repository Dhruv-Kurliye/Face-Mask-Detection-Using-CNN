# Face Mask Detection System

## 📌 Project Overview
This project is a **Deep Learning-based Face Mask Detection System** that classifies faces as **masked** or **unmasked** in real-time. The system leverages **VGG16** as a feature extractor using **transfer learning** and is implemented using **Keras** and **TensorFlow**. The model achieves **95% accuracy** on validation data and integrates **OpenCV** for real-time face detection and classification from live video streams.

## 🚀 Features
- **Deep Learning Model:** Uses **VGG16** as a feature extractor for mask detection.
- **Real-Time Detection:** Detects faces and classifies them as masked or unmasked in live video streams.
- **Transfer Learning:** Utilizes pre-trained VGG16 weights for improved accuracy.
- **Data Augmentation:** Enhances robustness with techniques like rotation, flipping, and zooming.
- **Optimization:** Uses **Adam optimizer**, dropout layers, and early stopping to prevent overfitting.

---

## 📂 Dataset
The dataset consists of images categorized into two classes:
- `Masked` - Faces wearing masks
- `Unmasked` - Faces without masks

### **Preprocessing Steps:**
1. **Image Resizing:** Resized images to `224x224` for VGG16 compatibility.
2. **Normalization:** Pixel values scaled to range `[0,1]`.
3. **Data Augmentation:** Applied random rotations, flips, and zooms.

## 🏗️ Model Architecture
- **Base Model:** `VGG16` (Pre-trained on ImageNet)
- **Fully Connected Layers:**
  - Dense layers with ReLU activation
  - Dropout layers to reduce overfitting
  - Final Softmax layer (2 classes: Masked, Unmasked)

---

## 🎥 Real-Time Face Mask Detection
This project uses **OpenCV** to capture live video and classify faces in real time.

### **Steps to Run Live Detection:**
1. Ensure a webcam is connected.
2. Run the following command:
   ```sh
   python detect_mask.py
   ```
3. The system will detect faces and classify them in real time.

---

## 📊 Results
- **Training Accuracy:** ~96%
- **Validation Accuracy:** ~95%
- **Loss Optimization:** Achieved through **Adam optimizer** and **early stopping**.

---

## 🤖 Technologies Used
- **Python**
- **TensorFlow & Keras**
- **VGG16 (Transfer Learning)**
- **OpenCV**
- **NumPy & Pandas**
- **Matplotlib (for visualization)**

---

## 💡 Future Improvements
- Support for **multiple face detection** in a single frame.
- **Mobile Deployment** using TensorFlow Lite.
- Integration with **Raspberry Pi** for IoT-based applications.
- Optimization for **edge devices**.

---

## 👨‍💻 Author
**Dhruv Kurliye**  
📧 Email: [kurliyedrk@gmail.com](mailto:kurliyedrk@gmail.com)  
🔗 GitHub: [Dhruv-Kurliye](https://github.com/Dhruv-Kurliye)  



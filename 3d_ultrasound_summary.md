
# 3D Ultrasound Reconstruction Using Deep Learning and Computer Vision

**Author**: Nihar Prakash Asare  
**Institution**: University at Buffalo – Robotics Program  
**Advisor**: Dr. Jun Xia  
**Project Duration**: Fall 2024  

---

## 🧠 Objective
Develop a 3D reconstruction system integrating **Ultrasound imaging**, **Optical Tracking**, and **Inertial Measurement Units (IMUs)** using Computer Vision and Deep Learning to improve non-invasive biomedical diagnostics.

---

## 🔧 Methodology
- **Data Acquisition**: Used a CONTEC ultrasound probe with NDI Polaris VICRA optical tracker and Yost Labs IMU. Synchronized 1000-frame wrist scans with timestamped sensor data.
- **Preprocessing Pipeline**:
  - Extracted frames from app-recorded videos using OpenCV
  - Matched IMU and Optical Tracker data with frames using a custom timestamp algorithm
  - Saved aligned multimodal data in `.npy` format for spatial mapping
- **3D Reconstruction**:
  - *Optical-based Reconstruction*: Normalized pose data used to reconstruct a smooth 3D volume via trilinear interpolation and Gaussian filtering
  - *IMU-based Prediction*: Built a deep learning architecture using **ResNet-50 + GRU** to model spatial-temporal relations from ultrasound images and Euler angles

---

## 📊 Results
- Achieved sub-millimeter 3D reconstruction accuracy using optical tracking
- Demonstrated early-stage success with deep learning-based IMU modeling
- Enabled automated 3D visualization of anatomical wrist structures from freehand probe motion

---

## ✅ Conclusion
The system integrates sensor fusion and machine learning for real-time, volumetric ultrasound imaging, providing a foundation for future research in robotic medical diagnostics and intraoperative guidance.

---


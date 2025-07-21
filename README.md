# anomaly-detection-of-Brainstem-glioma-using-Autoencoders


This project focuses on the detection of **Brainstem Gliomas (specifically Diffuse Intrinsic Pontine Gliomas - DIPG)** using **unsupervised anomaly detection** with Autoencoders. It aims to enhance tumor boundary detection and assist radiologists with early diagnosis from MRI and CT scans.

---

## 👥 Team Members
- Annesha Das (RA2211004010601)
- J Sai Siddharth (RA2211004010630)
- Manjusha M (RA2211004010637)
- **Guide**: Dr. Giriprasad S, Assistant Professor, Dept. of Electronics and Communication, SRM Institute of Science and Technology

---

## 📖 Introduction
Brainstem gliomas are difficult to diagnose early due to their deep-seated location, subtle symptoms, and complex anatomy. Manual segmentation is prone to errors and variability. This project develops an **AI-based anomaly detection model** using **Autoencoders** to identify tumors with greater speed, accuracy, and reproducibility.

---

## 🎯 Motivation & Objectives
### Motivation
- Manual segmentation is time-consuming and inconsistent.
- AI enhances accuracy and reduces human error.
- Early detection improves treatment outcomes.

### Objectives
- Develop an unsupervised Autoencoder-based anomaly detection model.
- Improve tumor boundary detection with attention mechanisms.
- Validate on real MRI and CT datasets.
- Optimize for real-time clinical applications.

---

## 📚 Literature Review Highlights
- **Challenges in Early Detection**: Subtle imaging characteristics, nonspecific symptoms, and anatomical constraints.
- **Need for Unsupervised Methods**: Due to scarce annotated datasets.
- **Autoencoders**: Train on healthy brain scans to detect anomalies via reconstruction error.

---

## 🏗️ System Workflow
1. **Input**: CT/MRI raw medical images
2. **Preprocessing**:
   - Grayscale conversion
   - Resizing to 256x256
   - CLAHE filtering for noise reduction
3. **Model**:
   - Convolutional Autoencoder (CNN-based)
   - Trained on healthy brain images
4. **Anomaly Detection**:
   - Compute Mean Squared Error (MSE) between original & reconstructed images
   - Threshold to classify healthy vs glioma
5. **Output**: Highlighted glioma regions for clinical interpretation

---

## 🔥 Why Autoencoder over U-Net?
| Feature                          | Autoencoder                      | U-Net                         |
|----------------------------------|------------------------------------|--------------------------------|
| Data Requirements                | Only healthy images               | Requires annotated tumor data |
| Rare Condition Detection         | Yes                               | Limited                        |
| Labeling Effort                  | Minimal                           | High                           |
| Flexibility                      | Works across modalities           | Needs retraining               |
| Subtle Anomaly Detection         | Excellent                         | May miss subtle anomalies      |
| Computational Efficiency         | Faster                            | More resource intensive        |

---

## 📊 Results
- ✅ **Improved detection accuracy**: Autoencoder effectively distinguishes glioma anomalies.
- ⏱️ **Fast localization**: Minimal human intervention required.
- ✨ **Visual precision**: Reconstruction error maps highlight glioma boundaries.
- 🔄 **Reduced dependency on manual annotation**.

---

## ⚡ Engineering Standards & Compliance
- **IEEE Standards**: AI in medical imaging
- **Data Privacy**: HIPAA & GDPR compliant
- **Medical Standards**: DICOM compatibility
- **Clinical Validation**: Aligns with FDA & CE guidelines

---

## 🚀 Future Work
- Implement **3D Autoencoders** for volumetric data
- Integrate **Attention Mechanisms** and multimodal MRI
- Expand validation across diverse datasets for clinical integration

---

## 💻 Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- Google Colab (for training & testing)

---

## 📂 Dataset
Healthy and glioma-affected brain MRI/CT scans (processed to grayscale and resized).  
*Note: Due to privacy concerns, raw datasets are not shared publicly.*

---

## 📎 References
1. Myronenko, A. *3D MRI Brain Tumor Segmentation Using Autoencoder Regularization*, BrainLes 2018.
2. Aswani & Menaka, *Dual Autoencoder Feature Optimization*, BMC Medical Imaging, 2021.
3. Chatterjee et al., *StRegA: Unsupervised Anomaly Detection*, Computers in Biology and Medicine, 2022.
4. Wen et al., *Deep Ensemble Framework for Glioma Segmentation*, Scientific Reports, 2025.

For full list: [See References in PPT](https://colab.research.google.com/drive/1MBSy_NWjpgLI6Suh-X5FfaoSbHrTyGp8#scrollTo=SCWgq1R3RetI)

---

## 📁 Project Structure

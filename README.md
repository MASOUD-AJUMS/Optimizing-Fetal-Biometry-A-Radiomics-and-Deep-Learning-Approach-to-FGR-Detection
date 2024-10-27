

```markdown
Optimizing Fetal Biometry: A Radiomics and Deep Learning Approach to FGR Detection

Introduction
This project presents an AI-based framework for the automated detection of fetal growth restriction (FGR), especially in low-resource settings. The goal is to ensure accurate abdominal circumference (AC) measurements through automated frame selection and segmentation, reducing dependency on skilled sonographers and improving access to quality prenatal care.

Project Objectives
- **Enhance accuracy in FGR detection**: Utilize deep learning and radiomics algorithms for accurate frame classification and segmentation.
- **Reduce dependency on skilled sonographers**: Automate the process of frame selection and segmentation.
- **Improve access to quality prenatal care**: Provide effective tools for accurate fetal biometry, especially in underserved regions.

Methods
The proposed framework consists of two main components: **radiomics-based frame classification** and **attention-based U-Net segmentation**.

1. **Frame Classification**: In the classification stage, ultrasound frames were analyzed to determine those optimal for AC measurement. Radiomic features were extracted, followed by feature selection. Multi-classifiers were trained on these selected features to distinguish optimal from non-optimal frames, achieving high accuracy.
2. **Segmentation**: The selected frames were then processed by an attention-based residual U-Net model to accurately delineate fetal abdominal boundaries. This model was trained over 150 epochs with a batch size of 16. Metrics like **Intersection over Union (IoU)**, **Dice score**, and **F1-score** were used to evaluate segmentation performance.

Results
- The radiomics-based classification system achieved **91% accuracy**, with **precision (0.89)** and **recall (0.96)**, ensuring the selection of high-quality frames for biometry.
- The attention-based U-Net model delivered excellent segmentation results, achieving **IoU of 0.95** and **F1-score of 0.99**. Minimal divergence between training and validation curves confirmed the model’s ability to generalize effectively across unseen data.

Conclusion
By providing an affordable and scalable tool for AC measurement, this framework can enhance early detection and management of FGR, especially in underserved regions, contributing to improved maternal and fetal health outcomes globally.

Prerequisites

To run this project, install the following:

- Python 3.7 or above
- Required libraries:
  - NumPy
  - Pandas
  - Scikit-Learn
  - TensorFlow or PyTorch
  - OpenCV
  - Matplotlib

You can install all prerequisites by running:

```bash
pip install -r requirements.txt
```

Project Setup

1. Clone this repository:

   ```bash
   git clone https://github.com/MASOUD-AJUMS/Optimizing-Fetal-Biometry-A-Radiomics-and-Deep-Learning-Approach-to-FGR-Detection.git
   cd Optimizing-Fetal-Biometry-A-Radiomics-and-Deep-Learning-Approach-to-FGR-Detection
   ```

2. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

3. Prepare the necessary data and place it in the specified directories.

Usage

You can run each part of the framework independently to suit your workflow or data availability. Here’s a breakdown of the main steps:

1. **Frame Classification**: To identify optimal frames for AC measurement, run the frame classification model. This will select the most suitable ultrasound frames for further processing.

   ```bash
   python Frame Classification Using Machine Learning.py

```

Folder Structure

- `data/`https://drive.google.com/file/d/1fuu0jpTh3FLOcfhDMefi_QAP2sqVy9IZ/view?usp=drive_link.
- `Frame Classification/`: Frame Classification Using Machine Learning.
- `Automated Segmentation/`Automated Segmentation of the Fetal Abdomen.

Contribution

Contributions are welcome! Please submit a Pull Request or raise Issues for any suggestions or improvements.

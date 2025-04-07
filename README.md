# Breast Cancer Detection using Convolutional Neural Networks (CNN)

Breast cancer is one of the leading causes of cancer-related deaths globally. Accurate diagnosis from hematoxylin and eosin (H&E)-stained images is challenging and often leads to inconsistent results among medical professionals. **Computer-Aided Diagnosis (CAD)** systems can significantly improve diagnostic efficiency and reduce human error. Traditional methods rely on handcrafted features, which are often limited by domain knowledge and scalability. This project leverages **deep learning**, specifically **Convolutional Neural Networks (CNNs)**, to address these challenges.

---

## 🧠 Project Overview
This project proposes a CNN-based approach for classifying H&E-stained breast biopsy images into:

- **Four Categories**:
  - Normal Tissue
  - Benign Lesion
  - In Situ Carcinoma
  - Invasive Carcinoma

- **Binary Classification**:
  - Carcinoma
  - Non-Carcinoma

Our architecture is designed to extract features across multiple scales, capturing both the micro-level cellular structure and macro-level tissue organization. The model achieves:

- **77.8% Accuracy** in four-class classification
- **95.6% Sensitivity** for cancer detection in binary classification

---

## 📁 Project Structure
```
.
├── BreastCancer.py                # Main script
├── model.h5                       # Pretrained model
├── my_image.jpg                   # Image for custom testing
├── /data/                         # Folder for preprocessed image data
│   ├── file1.npy
│   ├── file2.npy
│   └── ...
```

---

## 🔧 Requirements
Ensure you have **Python 3** installed.

### Python Libraries
Install the required libraries using pip:
```bash
pip install keras tensorflow pillow numpy
```

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/mishraShilpa-28/breast-cancer-detection.git
cd breast-cancer-detection
```

### 2. Prepare the Data
Download the preprocessed image data (provided separately) and place the `.npy` files in the project directory alongside the `BreastCancer.py` file.

### 3. Modify Hyperparameters *(Optional)*
In the first few lines of `BreastCancer.py`, modify the values between `#` markers to adjust the model's hyperparameters.

### 4. Run the Program
To start training or testing:
```bash
python BreastCancer.py
```
Follow the on-screen prompts to choose between:
- Training the model
- Testing the model
- Testing your own image

### 5. Testing Your Own Image
Place your test image in the same directory as `BreastCancer.py` and rename it to `my_image.jpg`. Then run the program and choose the test option.

---

## 🧪 Pretrained Model
A pretrained model is included (`model.h5`). You can use it to make predictions directly without retraining the network.

---

## 📊 Results
| Classification Type | Accuracy / Sensitivity |
|---------------------|------------------------|
| Four-Class          | 77.8% Accuracy         |
| Binary (Cancer)     | 95.6% Sensitivity      |

---

## 📜 License
This project is open-source and available under the MIT License.

---

## 🙌 Acknowledgements
Special thanks to researchers and contributors in the field of medical imaging and deep learning whose work made this project possible.


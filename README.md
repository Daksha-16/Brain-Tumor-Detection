
# 🧠 Brain Tumor Detection using Deep Learning (CNN)

A deep learning-based solution for binary classification of brain MRI images into Tumor and No Tumor categories. This project leverages Convolutional Neural Networks (CNNs) to assist in early detection of brain tumors from medical imaging.

![Brain Tumor Classification](https://github.com/Daksha-16/Brain-Tumor-Detection/blob/main/Brain.jpg)

---

 📝 Project Summary

This project applies computer vision and medical imaging techniques to classify brain MRI scans. Using TensorFlow and OpenCV, the model learns spatial features to predict whether a tumor is present.

🔍 Goal: Assist radiologists by providing fast, AI-based tumor detection.

📁 Dataset: Brain MRI scans (2 classes – Yes/No tumor)

🎯 Model Accuracy: ~82% on test data

---

 📂 Project Structure

```

Brain-Tumor-Detection/
│
├── brain\_tumor\_dataset/           # Dataset (not uploaded to GitHub)
│   ├── yes/                       # MRI images with tumors
│   └── no/                        # MRI images without tumors
│
├── Brain-tumor-detector.py        # Model training & evaluation script
├── Brain-tumor-probability.py     # Predict tumor probability for a single image
├── brain\_tumor\_model.h5           # Saved CNN model
├── requirements.txt               # Python dependencies
├── README.md                      # Project documentation
└── .gitignore                     # Ignore unnecessary files

````

---

 💡 Key Features

- Binary classification: Tumor vs. No Tumor
- CNN-based deep learning architecture
- Model saves as `.h5` for future predictions
- Image preprocessing using OpenCV
- Predict probability of tumor from any custom image

---

 ⚙️ Tech Stack

| Technology    | Purpose                  |
|---------------|--------------------------|
| Python        | Core programming         |
| TensorFlow/Keras | Deep learning model      |
| OpenCV        | Image loading/preprocessing |
| Scikit-learn  | Data splitting & evaluation |
| NumPy         | Numerical operations      |

---

 🚀 How to Run the Project

# 🔧 1. Clone the Repository

```bash
git clone https://github.com/Daksha-16/Brain-Tumor-Detection.git
cd Brain-Tumor-Detection
````

# 🧪 2. Install Dependencies

```bash
pip install -r requirements.txt
```

# 📁 3. Prepare Dataset

Place MRI images in the following structure:

```
brain_tumor_dataset/
├── yes/
├── no/
```

(Due to size, dataset is not uploaded — use public datasets from Kaggle or similar.)

---

# 🧠 4. Train the CNN Model

```bash
python Brain-tumor-detector.py
```

✅ The script will:

 Load and preprocess images
 Train a CNN model
 Save it as `brain_tumor_model.h5`

---

# 🔍 5. Predict Tumor from Image

```bash
python Brain-tumor-probability.py
```

Result:

```bash
Probability of the image being a tumor: 90.26%
```

---

 📈 Model Performance

| Metric       | Value |
| ------------ | ----- |
| Accuracy     | \~82% |
| Epochs       | 10    |
| Architecture | CNN   |

Model performance may vary based on dataset size, augmentation, and tuning.


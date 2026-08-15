# 🍕 Food Recognition using EfficientNetB0

A deep learning-based **Food Recognition System** that classifies food images into **101 different food categories** using transfer learning with **EfficientNetB0**.

## 🚀 Project Overview

This project uses a pretrained **EfficientNetB0** model with ImageNet weights to recognize different types of food from images.

The model was trained using the **Food-101 dataset**, containing 101 food categories and 101,000 images.

The project demonstrates:

* Image classification
* Transfer learning
* Deep learning with TensorFlow/Keras
* Food image preprocessing
* Model training and evaluation
* Real-world image prediction

## 📊 Dataset

The project uses the **Food-101 dataset**.

* **Food categories:** 101
* **Total images:** 101,000
* **Training images:** 80,800
* **Validation images:** 20,200
* **Images per category:** 1,000

Dataset structure:

```text
food-101/
├── images/
│   ├── apple_pie/
│   ├── pizza/
│   ├── burger/
│   └── ...
└── meta/
```

## 🧠 Model

The project uses **EfficientNetB0** with pretrained ImageNet weights.

### Architecture

```text
Input Image
     ↓
EfficientNetB0
     ↓
Global Average Pooling
     ↓
Dropout (0.3)
     ↓
Dense Layer (101 classes)
     ↓
Softmax
     ↓
Predicted Food Class
```

The pretrained EfficientNetB0 layers were initially frozen and a new classification layer was added for the 101 food categories.

## 📈 Results

The model was trained for 3 epochs using a reduced training subset for faster experimentation on CPU.

| Metric              | Result |
| ------------------- | -----: |
| Food Classes        |    101 |
| Training Accuracy   | 63.36% |
| Validation Accuracy | 59.42% |
| Validation Loss     | 1.6239 |

### Example Prediction

```text
Input: Pizza Image
Prediction: Pizza
Confidence: 54.81%
```

## 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* EfficientNetB0
* NumPy
* Matplotlib
* OpenCV
* Jupyter Notebook
* VS Code

## 📁 Project Structure

```text
PRODIGY_ML_05/
│
├── notebook/
│   ├── food_recognition.ipynb
│   └── pizza.jpg
│
├── food_recognition_model.keras
├── README.md
└── requirements.txt
```

> The Food-101 dataset is not included in this repository because of its large size.

## ⚙️ Installation

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd PRODIGY_ML_05
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ How to Run

1. Download the Food-101 dataset.
2. Place the dataset inside the project's `dataset/food-101/` directory.
3. Open the Jupyter notebook:

```text
notebook/food_recognition.ipynb
```

4. Run the notebook cells.
5. Train the EfficientNetB0 model.
6. Provide a food image for prediction.
7. The model will return the predicted food category and confidence score.

## 🔮 Future Improvements

* Train on the complete Food-101 dataset.
* Increase the number of training epochs.
* Fine-tune the pretrained EfficientNet layers.
* Use GPU acceleration.
* Improve validation accuracy.
* Add a web interface using Streamlit or Flask.
* Add calorie estimation for recognized foods.
* Deploy the model as a web application or API.

## 👨‍💻 Author

**Krishna**

B.Tech CSE — AI/ML

## ⭐ Project Highlights

This project demonstrates practical experience with:

**Deep Learning • Transfer Learning • Computer Vision • Image Classification • TensorFlow • Keras • EfficientNet**

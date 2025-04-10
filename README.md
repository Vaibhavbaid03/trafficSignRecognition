# Traffic Sign Recognition with CNN and OpenCV

This project implements a real-time **Traffic Sign Recognition System** using a **Convolutional Neural Network (CNN)** in TensorFlow/Keras and OpenCV for preprocessing and live video capture.

---

## Features

- Loads and preprocesses traffic sign images
- Builds a custom CNN for classification
- Augments data for better generalization
- Evaluates and visualizes model performance
- Real-time recognition using webcam

---

## Project Structure

```
├── myData/                  # Folder containing subfolders of image classes
├── labels.csv               # Mapping of class indices to label names
├── model_trained.p          # Pickled trained model
├── train.py                 # Full training pipeline
├── recognize.py             # Real-time traffic sign recognition
└── README.md                # You are here
```

---

##  Requirements

Install dependencies:

```bash
pip install numpy opencv-python tensorflow keras matplotlib pandas scikit-learn
```

---

## Training the Model

Run the training script to:
- Load and preprocess the dataset
- Split into train/validation/test sets
- Train a CNN with image augmentation
- Save the trained model using `pickle`

```bash
python train.py
```

---

## Real-Time Recognition

Once trained, run the webcam recognition script:

```bash
python recognize.py
```

Make sure `model_trained.p` is in the same directory.

---

## Author

**Vaibhav Baid**  
B.E. in Artificial Intelligence & Data Science  
Project developed as part of coursework + personal interest.

---

##  Notes

- `imageDimensions` are set to `(32, 32, 3)`; change accordingly if dataset differs.
- Model uses grayscale preprocessing and histogram equalization.
- Threshold for real-time prediction is customizable (`threshold = 0.75`).



# face_mask_detection_using_CNN

##🧠 Project Description

Face Mask Detection using CNN is a deep learning–based computer vision project that automatically detects whether a person is wearing a face mask or not in real time. It uses a Convolutional Neural Network (CNN) model trained on images of faces with and without masks to classify new input images or video frames.

## Motivation
Amid the ongoing COVID-19 pandemic, there are no efficient face mask detection applications which are now in high demand for transportation means, densely populated areas, residential districts, large-scale manufacturers and other enterprises to ensure safety. The absence of large datasets of ‘with_mask’ images has made this task cumbersome and challenging. 

## ⚙️ How It Works

- Dataset Preparation:
The dataset is divided into two categories — with_mask and without_mask.

- Model Training:
A CNN model (built using TensorFlow/Keras) is trained to learn distinguishing facial features between masked and unmasked faces.

- Detection Phase:

The model takes live video or image input.

Detects faces using OpenCV’s Haar cascades or DNN-based face detection.

Classifies each detected face as “Mask” or “No Mask.”

## Prerequisites
Install the following before starting:
- Python 3.x
- tensorflow
- keras
- opencv-python
- numpy
- sklearn
- matplotlib

## Installation
1. Clone the repository:
   ```
   git clone https://github.com/chandrika203/face_mask_detection_using_CNN.git
   ```
2. Change to project directory:
   ```
   cd face_mask_detection_using_CNN
   ```
3. Install requirements:
   ```
   pip install -r requirements.txt
   ```

## Dataset
The dataset used can be downloaded here – [https://www.kaggle.com/datasets/omkargurav/face-mask-dataset]

It consists of images in two categories:
- `with_mask` – images of faces wearing a mask
- `without_mask` – images of faces without a mask

## Working
Run the following to train and test the model:

### 1. Train the Model
```
python train_mask_detector.py --dataset dataset
```

### 2. Detect Mask in an Image
```
python detect_mask_image.py --image images/sample.jpg
```

### 3. Detect Mask in Real-time Video Stream
```
python detect_mask_video.py
```

## Results
The trained model achieved approximately **98% accuracy** in mask detection.
Accuracy and loss training curves plot provided inside the project.

## Features
- Detect face masks in real time using webcam.
- Detect in static images or video streams.
- Efficient architecture suitable for embedded devices.

## Use Cases
- Deployment in airports, railway stations, schools, offices, and public places to ensure mask compliance.
- Security systems to automatically issue alerts when someone is not wearing a mask.

## Contributing
Contributions, issues, and feature requests are welcome!
Check the project's issues and pull requests pages for more info.


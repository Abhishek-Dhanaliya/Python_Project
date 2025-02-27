**Face Recognition System**

# Project Overview

This Face Recognition System is designed to detect, store, and recognize human faces using OpenCV and Python. 
The project captures face images from a webcam, stores them in a dataset, and then uses a trained model to recognize faces in real-time.

# Requirements

Ensure you have the following installed before running the project:

Python (latest version) → https://www.python.org/downloads/

Required Python Packages:

opencv-python

opencv-contrib-python

numpy

You can install them using:

// pip install opencv-python opencv-contrib-python numpy

# Installation and Setup

Clone or download the project files.

Open the project in PyCharm or any Python IDE.

Ensure that the required libraries are installed.

Modify the dataset and cascade classifier paths as per your system:

Dataset Path: Dataset.py (Line 6 & 30), Detection.py (Line 6)

Haar Cascade Path: Dataset.py (Line 4), Detection.py (Line 25)

# How to Run the Project

-> Step 1: Collect Face Samples

Run Dataset.py to capture and store face images.

This will detect faces, convert them to grayscale, and save them in the dataset folder.

// python Dataset.py

-> Step 2: Train the Model

The face images are used to train an LBPH (Local Binary Patterns Histogram) model for recognition.

This step is performed within Detection.py.

-> Step 3: Recognize Faces

Run Detection.py to start the recognition process.

The system will classify faces as "Known" or "Unknown" based on the trained dataset.

// python Detection.py

# File Descriptions

// Dataset.py

Captures face images from the webcam.

Crops and converts faces to grayscale.

Saves the images to a specified directory.

// Detection.py

Trains an LBPH model using collected face samples.

Uses OpenCV's Haar Cascade Classifier to detect faces.

Recognizes faces in real-time.

# Technologies Used

Programming Language: Python

Libraries: OpenCV, NumPy

Algorithm: LBPH (Local Binary Patterns Histogram)

IDE: PyCharm, VScode

Notes

Ensure the dataset is collected before running face recognition.

Modify file paths accordingly.

Use cv2.imshow() for debugging and viewing face captures.

Acknowledgments

This project was developed as part of a Face Recognition System using Python and OpenCV.

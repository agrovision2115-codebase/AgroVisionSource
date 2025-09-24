Plant Disease Detection & Treatment

A PyTorch-based model to identify plant diseases from leaf images, estimate infection severity, and provide treatment recommendations with dosage.

Features

Detects 38 plant disease classes (including healthy leaves).
Estimates infection severity: Mild, Moderate, Severe.
Provides treatment suggestions with dosage.
Quick prediction on single images.

Setup
Requirements

Python 3.9+
PyTorch
torchvision
Pillow
numpy

Install dependencies:

pip install torch torchvision pillow numpy

Model

Place the trained model pd2se_model.pth in the working directory.

Usage

Place a leaf image in the directory, e.g., test_leaf.jpg.
Run the predictor:
python predict.py


Example output:

Disease: Tomato Leaf Mold | Infection Level: Moderate | Treatment: Apply copper-based fungicide; 2 ml per liter of water

Notes

Only works with clear leaf images.
For diseases not in the treatment dictionary, consult local guidelines.
Model expects RGB images of size 224x224.

Future Improvements

Expand treatment dictionary to all 38 classes.
Add batch prediction for multiple images.
Create web or mobile interface for field use.

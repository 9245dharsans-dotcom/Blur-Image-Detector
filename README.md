# Blur Image Detector 📷
A deep learning model that detects whether a photo is sharp or blurry using CNN and MobileNetV2 transfer learning.

## What it does
Classifies images as **sharp** or **blurry** — useful for automatically cleaning up photo libraries by removing low quality images.

## Model
- Architecture: MobileNetV2 (Transfer Learning)
- Dataset: Custom dataset of sharp and blurry images
- Accuracy: **91.43%**
- Tested on real phone photos

## Tech Stack
- Python
- TensorFlow / Keras
- MobileNetV2 (pretrained on ImageNet)
- Google Colab

## How to run
1. Open `blur_image_detection.ipynb` in Google Colab
2. Run all cells in order
3. Test on your own images in the final cell

## Results
The model successfully distinguishes sharp vs blurry images with 91.43% accuracy on the test set.

# Blur Image Detector 📷
A deep learning model that detects whether a photo is sharp or blurry using CNN and MobileNetV2 transfer learning.

## What it does
Classifies images as **sharp** or **blurry** — useful for automatically cleaning up photo libraries by removing low quality images.

## Model
- Architecture: MobileNetV2 (Transfer Learning)
- Dataset: Blur Dataset (Kaggle) — 350 sharp, 350 defocused-blur, and 350 motion-blur images. Defocused-     blur and motion-blur were merged into a single "blurry" class, producing a binary dataset of 350 sharp     and 700 blurry images (1,050 total)
- Accuracy: **91.43%**
- Tested on real phone photos

## Additional Experiments
See `finetuning_experiments.ipynb` for a comparison of feature extraction 
vs. fine-tuning strategies on this dataset. Fine-tuning was found to 
underperform feature extraction due to the small dataset size — 
see the full report for detailed analysis.

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

📄 Published report: https://doi.org/10.5281/zenodo.20833021


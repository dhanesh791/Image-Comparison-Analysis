Image Alignment and Change Detection

Overview

This project aligns two ortho-rectified images, detects changes between them, and classifies the changes using a Convolutional Neural Network (CNN). The primary goal is to segment and classify different changes effectively while correcting for environmental factors such as lighting and contrast variations.

Features

Image Preprocessing: Enhances contrast and corrects environmental factors.

Change Detection: Uses image differencing and morphological operations.

Pixel-wise Classification: Trains a CNN to classify changed pixels.

Segmentation & Visualization: Creates heatmaps and outlines detected changes.

Dependencies

Ensure you have the following dependencies installed:

pip install numpy opencv-python matplotlib scikit-image tensorflow scikit-learn

File Structure

image_alignment.py: Main script for image alignment and change detection.

A (2).png, B (2).png: Sample images for testing.

Usage

Place the images in the working directory.

Run the script:

python image_alignment.py

The script will display:

A heatmap representing detected changes.

An image with segmented change contours.

Model Training

The CNN classifier takes pixel-wise data and trains on image differences.

It uses a simple convolutional architecture with dropout for regularization.

The trained model predicts change classifications for each pixel.

Output

Change Heatmap: Highlights areas of detected changes.

Segmented Image: Outlines classified changes on the original image.

Future Enhancements

Implement a more advanced deep learning model (e.g., U-Net) for better segmentation.

Introduce multi-class classification for different change types.

Use pre-trained models for improved accuracy.

Author

Developed by [Dhaneshwaran Ponnurangam]

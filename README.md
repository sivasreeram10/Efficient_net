# Efficient_net
banana-disease-detection-efficientnet
EfficientNet-Based Banana Plant Disease Detection
Overview
This project implements EfficientNetB0, a highly optimized and scalable deep learning model, for detecting banana plant diseases using leaf images. EfficientNet provides a balance between accuracy and computational efficiency, making it suitable for real-time applications.

Features
✅ Highly Accurate – EfficientNet provides state-of-the-art performance with fewer parameters.
✅ Optimized for Mobile & Edge Devices – Can be deployed on IoT-based disease monitoring systems.
✅ Transfer Learning – Uses a pretrained ImageNet model to extract disease features.
✅ Real-Time Detection – Processes images efficiently with minimal computational overhead.

Dataset
The model is trained on a dataset containing healthy and diseased banana leaf images. Categories include:

Healthy Leaves
Diseased Leaves (e.g., Fusarium Wilt, Black Sigatoka, Banana Bunchy Top Virus, etc.)
Workflow
1. Data Preprocessing
Load high-resolution banana leaf images.
Resize images to 224×224 pixels (EfficientNetB0 input size).
Apply image augmentation (rotation, flipping, zooming) for better generalization.
2. Model Architecture (EfficientNetB0)
EfficientNet enhances feature extraction by using:

Compound Scaling – Balances depth, width, and resolution for better accuracy.
Inverted Bottleneck Layers – Improve efficiency while retaining features.
Swish Activation – Enhances non-linearity and improves performance.
Batch Normalization – Stabilizes and accelerates training.
3. Training the Model
Loss Function: Categorical Cross-Entropy
Optimizer: Adam
Evaluation Metrics: Accuracy & Loss
4. Classification & Prediction
The trained model classifies banana leaf images into healthy or diseased categories.
Provides confidence scores for predictions.
Can be deployed on mobile apps, web platforms, and IoT-based monitoring systems.
Installation
Clone the repository:
git clone https://github.com/yourusername/efficientnet-banana-disease-detection.git
cd efficientnet-banana-disease-detection
Install dependencies: bash Copy Edit pip install -r requirements.txt Train the model: bash Copy Edit python train.py Run inference on a sample image: bash Copy Edit python predict.py --image sample_leaf.jpg Results Achieved high accuracy in detecting banana plant diseases. Lower computational cost compared to traditional CNNs. Future Improvements 🔹 Extend dataset for more banana plant diseases. 🔹 Optimize for real-time edge computing and drone-based analysis. 🔹 Deploy on IoT devices for smart farming applications.

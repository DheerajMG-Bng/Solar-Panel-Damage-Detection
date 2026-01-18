## Solar Panel Defect Detection using Deep Learning
 
 Project Summary
-------------------------

Built an automated solar panel inspection system using deep learning

Eliminates manual inspection, which is slow and error-prone

Uses CNNs, Transfer Learning, and Ensemble Learning

Final output is a single, clear defect label for each solar panel image


# What Problem This Project Solves

Manual inspection of solar panels is:

Time-consuming

Costly

Inconsistent

Undetected defects reduce:

Energy efficiency

Panel lifespan

This project provides a scalable, intelligent, image-based solution

## What I Learned (Key Takeaways)

Real-world dataset preparation & cleaning

Designing end-to-end ML pipelines

Applying transfer learning effectively

Binary vs Multi-Class classification design

Ensemble learning for robustness

Model evaluation and comparison


# Technologies & Tools Used

Programming: Python

Platform: Google Colab

Frameworks: TensorFlow, Keras

Libraries: NumPy, Matplotlib

Concepts: CNN, Transfer Learning, Ensemble Learning

# Models Used

ResNet (ResNet50 variants)

VGG (VGG16 / VGG19)

MobileNet

All models are ImageNet pretrained

Custom dense layers added for defect detection

# Dataset

Source: Kaggle

Link:
 https://www.kaggle.com/datasets/pythonafroz/solar-panel-images

Contains solar panel images categorized as:

Clean

Bird-drop

Dusty

Electrical-damage

Physical-Damage

Snow-Covered

# Final Inference Pipeline (CORE LOGIC)

Input: Solar panel image

Stage 1 – Binary Classification (Ensemble CNN):

Determines Defective vs Non-Defective

Decision Logic:

Non-Defective → Clean (Final Output)

Defective → Sent to Multi-Class CNN

Stage 2 – Multi-Class Classification:

Identifies the exact defect type

Final Output (Single Label):

Clean

Bird-drop

Dusty

Electrical-damage

Physical-Damage

Snow-Covered

# Why This Approach is Strong

Two-stage pipeline → higher accuracy

Ensemble models → reduced bias & false predictions

Clean panels exit early → efficient computation

Defect labels map directly to real maintenance categories

Designed like a real industrial inspection system


# Methodology

Collected labeled solar panel images

Cleaned and organized dataset

Applied image preprocessing & augmentation

Trained binary CNN for defect detection

Compared multiple CNN architectures

Applied ensemble learning for optimization

Trained multi-class CNN for defect type detection

Generated final human-readable output

# What Makes This Project Unique

✔️ Uses ensemble learning, not a single model

✔️ Two-stage intelligent decision system

✔️ Clean and modular pipeline design

✔️ Research-oriented implementation

✔️ Real-world industrial relevance

✔️ Professional GitHub structure

# Final Output 

The system automatically detects whether a solar panel is defective using an ensemble CNN model and, if defective, identifies the exact defect type using a multi-class CNN.
The system automatically detects whether a solar panel is defective using an ensemble CNN model and, if defective, identifies the exact defect type using a multi-class CNN.

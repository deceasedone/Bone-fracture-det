# Bone Fracture Detection
This repository contains the implementation of an automated bone fracture detection system using deep learning techniques. The project employs a two-step approach with the ResNet50 architecture to enhance early diagnosis and support clinical decision-making.

# Project Overview
Bone fractures require prompt diagnosis; however, manual X-ray analysis is often challenging and resource-intensive, particularly in rural settings. This project tackles these issues by:

Classifying Bone Type: Using a CNN to accurately identify the bone (elbow, hand, or shoulder) with a 99.46% accuracy rate.
Detecting Fractures: Applying specialized models on the classified bone images to detect fractures, achieving an overall accuracy of 93.9%.
Motivation
Healthcare Accessibility: Addressing the shortage of expert radiologists in underdeveloped regions.
Cost-Effective Diagnosis: Utilizing affordable X-ray imaging to reduce dependency on expensive diagnostic modalities like CT and MRI.
Improved Accuracy: Automating fracture detection to lower diagnostic errors and streamline clinical workflows.
Dataset
The model is trained on the MURA dataset, which comprises over 20,000 X-ray images categorized by bone type and condition (normal vs. fractured).

# Methodology
Data Preprocessing:
Employed data augmentation techniques (e.g., horizontal flipping) to enhance dataset diversity.
Normalized and resized images to suit the model's input requirements.
Model Architecture:
Utilized ResNet50 for its robust feature extraction capabilities.
Implemented a two-step classification process: initial bone type detection followed by targeted fracture identification.
Training & Evaluation:
Achieved 99.46% accuracy in classifying bone types.
Recorded fracture detection accuracies of 83.02% (elbow), 85.12% (shoulder), and 80.31% (hand), culminating in an overall testing accuracy of 93.94%.

Jupyter notebooks for interactive model training and evaluation.
Python scripts for data preprocessing, model training, and performance visualization.
Detailed logs and graphs to track training progress and assess model performance.
Results & Analysis
The model demonstrates a robust performance in both bone classification and fracture detection tasks. The two-step process significantly enhances diagnostic accuracy, making it a viable tool for supporting radiologists in clinical environments.

# Future Work
Ensemble Modeling: Integrate additional architectures (e.g., Vision Transformers) to further boost detection accuracy.
Web App Integration: Develop an interactive interface for real-time fracture detection and report generation.
Dataset Expansion: Augment the dataset with more diverse imaging modalities to improve model generalization.

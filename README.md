# Fashion MNIST Image Classification with CNNs  
**Project By:** Ashkan Alinaghian, Arian PourEsmaeili, MohammadMahdi Khorsandpour  
**Date:** April 2025  

## Project Description  
This project implements and compares **three convolutional neural networks (CNNs)** for classifying clothing items in the Fashion MNIST dataset. We explore transfer learning, model complexity, and robustness to IIIF-annotated data distortions.  

**Key Objectives:**  
- Compare **transfer learning** (MNIST-pretrained) vs. **scratch-trained** vs. **deep CNNs** with advanced regularization.  
- Evaluate model generalization on IIIF-annotated samples and cross-dataset (MNIST digits).  
- Analyze misclassification patterns using confusion matrices and qualitative error analysis.  

**Methods & Tools:**  
- **Models:**  
  - Transfer Model (MNIST-pretrained feature extractor)  
  - Scratch Model (custom 4-layer CNN)  
  - Deep Model (BatchNorm, Dropout, Global Average Pooling)  
- **Techniques:** Data augmentation, class weighting, cross-validation, Adam/SGD optimization.  
- **Tools:** TensorFlow/Keras, IIIF Workbench for annotation, scikit-learn for evaluation.  

**Key Results:**  
- **Deep Model Achieved 91.3% Test Accuracy** (vs. 90.6% Scratch, 86.2% Transfer).  
- **IIIF Preprocessing Caused 20-30% Accuracy Drops** due to resizing artifacts.  
- **Shirts/Coats/Pullovers** were most error-prone (e.g., 25% misclassification rate for shirts).  
- **Cross-Dataset Generalization Failed** (10-12% accuracy on MNIST digits).  

**Conclusion:** Custom CNNs outperform ResNet18/LeNet5 on Fashion MNIST but remain sensitive to IIIF distortions. 

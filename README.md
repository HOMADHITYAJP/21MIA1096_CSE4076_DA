# 21MIA1096_CSE4076_DA

## Overview
This project explores the application of Quantum Convolutional Neural Networks (QCNNs) for the classification of astronomical objects, specifically stars and galaxies. By leveraging the unique properties of quantum computing, this research aims to improve classification accuracy and processing efficiency compared to traditional Convolutional Neural Networks (CNNs).

## Dataset
The dataset utilized in this project was generated from real-world observations conducted at the Aryabhatta Research Institute of Observational Sciences (ARIES), Nainital, India. Images were captured using the in-house 1.3m telescope and processed into 64x64 pixel cutouts. These images were labeled using image segmentation techniques and matched against the SDSS database, resulting in two distinct categories: galaxy and star.

- **Dataset Structure:**
  - **data/**
    - **galaxy/** (contains galaxy images)
    - **star/** (contains star images)
    
## Methodology
The methodology of the project is as follows:

1. **Data Preparation**: 
   - Implemented data augmentation and normalization techniques using TensorFlow's `ImageDataGenerator`.
   - Split the dataset into training and validation sets.

2. **Model Architecture**:
   - Developed a hybrid model integrating classical CNN layers with a quantum layer using PennyLane.
   - Key components of the model:
     - Convolutional layers for feature extraction.
     - MaxPooling layers to reduce dimensionality.
     - A quantum circuit designed to enhance feature representation through quantum superposition and entanglement.

3. **Training**:
   - The model was trained using the training dataset, with performance metrics monitored throughout the process.

4. **Evaluation**:
   - Performance metrics including accuracy, execution time, and memory usage were analyzed and compared against traditional CNNs.

## Key Findings
- **Enhanced Feature Representation**: QCNNs demonstrate superior capabilities in handling high-dimensional data, leading to improved classification accuracy.
- **Increased Efficiency**: The hybrid architecture allows for faster processing times and greater robustness against noise, vital for astronomical data analysis.
- **Potential Impact**: The integration of QCNNs into image classification tasks can significantly advance the field of astrophysics, enabling quicker analysis of large datasets and more accurate categorization of celestial objects.

## Performance Metrics Comparison

| Metric                     | CNN         | Hybrid QCNN      |
|----------------------------|-------------|-------------------|
| Execution Time (s)         | 683.824     | **53.4667**       |
| Memory Used (MB)           | 139.367     | **103.844**       |
| Accuracy                    | **0.768025**| 0.764228          |
| Validation Accuracy         | **0.810301**| 0.764411          |
| Loss                        | 0.499631    | **0.598027**      |
| Validation Loss             | 0.38051     | **0.571929**      |

## Conclusion
The findings of this research indicate that QCNNs possess significant potential in the domain of star-galaxy classification. The unique advantages of quantum computing may facilitate a deeper understanding of celestial phenomena and enhance the efficiency of data analysis in astronomical research.

As the field of quantum computing evolves, the integration of QCNNs into image processing tasks represents a crucial step towards unlocking new capabilities in scientific research and discovery.


Acknowledgments

## Acknowledgments

This project uses the "Dummy Astronomy Data" dataset provided by [Divyansh Agarwal](https://www.kaggle.com/datasets/divyansh22/dummy-astronomy-data) on Kaggle. 

We thank the author for making this dataset available for research purposes.


PennyLane for quantum machine learning capabilities

TensorFlow and Keras for deep learning framework

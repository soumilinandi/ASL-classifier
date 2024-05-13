# ASL Classifier

## Overview

This repository contains the implementation of a deep learning model for real-time interpretation of American Sign Language (ASL) from video data using a novel architecture that combines Transformer models with TensorFlow Lite. Our system processes both spatial and temporal features of ASL gestures, focusing on accessibility enhancements for the deaf and hard-of-hearing community.

## Project Details

### Authors

- Kunal Thadani
- Sakshi Goenka
- Soumili Nandi

### Abstract

The project uses advanced deep learning techniques to interpret ASL by processing video data with a hybrid approach that integrates Transformers and custom attention mechanisms. By leveraging extensive data preprocessing and robust Attention models, our goal is to improve communication tools for inclusivity.

### Problem Statement

Automated interpretation of sign language presents challenges such as gesture variability and limited data availability, leading to significant communication barriers. Our project addresses these by focusing on gesture recognition, variability and adaptability, and enriching training data.

### Dataset

The dataset used is from the Google-hosted Kaggle competition ["Isolated Sign Language Recognition"](https://www.kaggle.com/competitions/asl-signs). It includes landmark data obtained via MediaPipe, mapped to ASL signs, with extensive metadata for training robust models.

### Architecture

The core architecture involves:
- **Landmark Models**: Utilizing MediaPipe Holistic for generating comprehensive sets of landmarks.
- **Normalization and Dominant Hand Correction**: Adjusting data based on the detected dominant hand.
- **Embedding Layers**: Robust feature representation using dense layers.
- **Transformer Blocks**: Handling sequence processing for gesture recognition.
- **Pooling and Classification**: Final gesture classification using a softmax layer.

## Methodology

1. **Data Preparation**: Normalization and adjustment based on the dominant hand.
2. **Model Training**: Employing techniques like random masking and data augmentation for robustness.
3. **Validation and Evaluation**: Continuous performance evaluation during training using a separate validation set.

## Results

The model achieves a validation accuracy of approximately 74%, indicating strong potential for real-time applications in ASL interpretation.

## Installation and Usage

Clone this repository and install the required packages:

```bash
git clone https://github.com/soumilinandi/ASL-classifier
cd ASL-classifier
pip install -r requirements.txt
```

Run the main script to start the training process:

```bash
python train.py
```

## Acknowledgments

- Thanks to Google for providing the dataset on Kaggle.
- Special thanks to previous seminal works by Starner, Pentland, Cui et al., and others in the field of gesture recognition.

## Contributing

Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change. Please ensure to update tests as appropriate.

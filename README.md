# Komura: Confident Voices Matter

**Empowering Minds: A Holistic Approach to Education and Personal Development**

Komura is an innovative mobile application designed to help users improve their public speaking skills. By leveraging machine learning techniques, the app provides real-time feedback on filler words, speaking pace, articulation, and body language, enabling users to develop confidence and master their presentation skills.

---

## Project Overview

Public speaking remains a global challenge, with 75% of people experiencing glossophobia. Komura addresses this challenge by analyzing speech patterns and body language to provide actionable insights. By improving presentation style with live scoring and detailed analysis, users can grow into confident and effective communicators.

---

## Features

- **Real-time Feedback**: Provides analysis and scoring for:
  - Filler words
  - Speech speed
  - Articulation
  - Body language
- **Speech Confidence Analysis**: Utilizes machine learning to evaluate user confidence based on input features.
- **Intelligent Insights**: Uses audio and posture recognition for holistic public speaking improvement.
- **Mobile Integration**: Deploys a lightweight TFLite model for Android, ensuring smooth and efficient user experience.

---

## Project Workflow

### 1. **Dataset Preparation**
- Source: Audio and body language datasets collected and preprocessed for model training.
- Preprocessing: Tokenization, sequence padding, and augmentation with simulated filler words.

### 2. **Model Training**
- **Text Analysis Model**: Binary classification using Bi-LSTM layers for confidence prediction.
- **Feature Engineering**:
  - Counting filler words, connectors, and calculating speech duration.
  - Estimating confidence levels using calculated features.
- Fine-tuned using TensorFlow with early stopping and regularization.

### 3. **Mobile Deployment**
- Converted trained model to TensorFlow Lite for integration with Android apps.
- Utilized Kotlin and Jetpack Compose for UI/UX development.

---

## Tech Stack

- **Machine Learning**:
  - TensorFlow, Keras, NumPy, Pandas, OpenCV
- **Mobile Development**:
  - Android Studio, Kotlin, Jetpack Compose
- **Cloud**:
  - Google App Engine, Cloud SQL, Cloud Storage
- **Tools**:
  - Jupyter Notebook, Visual Studio Code, Flask, CameraX, Figma, GitHub

---

## Model Training Pipeline

1. **Dataset Processing**:
   - Tokenized and padded transcripts for text feature extraction.
   - Introduced variability with filler words and meaningless connectors.
2. **Model Architecture**:
   - Embedding layer for text representation.
   - Bidirectional LSTMs for sequential data processing.
   - Dense layers with regularization for binary classification.
3. **Training**:
   - Split dataset into training and testing sets.
   - Applied exponential learning rate decay and early stopping.
4. **Evaluation**:
   - Metrics: Accuracy, ROC-AUC, confusion matrix, classification report.
   - Visualized performance with loss and accuracy plots.

---

## How to Use

### Requirements
- Python 3.8+
- TensorFlow 2.5+
- Android Studio for app deployment

### Steps
1. **Clone Repository**:
   ```bash
   git clone <(https://github.com/presentation-app-capstone-bangkit)>
   cd <presentation-app-capstone-bangkit>

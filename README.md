# Handwriting Recognition

This project focuses on developing a system for recognizing text in handwritten images. It involves preprocessing the data to convert text labels into a numerical format and training neural networks for text recognition tasks.

## Key Components:

### Data Label Preprocessing:

- **Character Set and Constants:** Define the set of valid characters, maximum input label length, and other constants.
- **Label-to-Number Conversion:** Convert text labels into a numerical representation for training.
- **Number-to-Label Conversion:** Convert numerical representations back into text labels for evaluation.

### Convolutional Recurrent Neural Network (CRNN) Architecture:

- **Input Layer:** Accept grayscale images with dimensions of 256x64 pixels.
- **Convolutional Layers:** Apply convolutional filters and pooling operations for feature extraction.
- **Reshape Layer:** Reshape the output of convolutional layers for sequence processing.
- **Bidirectional LSTM Layers:** Utilize bidirectional LSTM layers for sequence modeling.
- **Output Layer:** Output layer with softmax activation for character prediction.

### Training and Evaluation:

- **CTC Loss Calculation:** Compute the Connectionist Temporal Classification (CTC) loss between predicted and true labels.
- **Training the Model:** Train the CRNN model using preprocessed data and evaluate its performance.
- **Evaluation Metrics:** Assess the model's performance using character-level accuracy and other metrics.

## Project Goals:

- Achieve high accuracy in recognizing handwritten text.
- Develop a robust system capable of handling various handwriting styles and conditions.
- Explore techniques for improving model performance and efficiency.

## Usage:

1. **Data Preprocessing:** Preprocess handwritten images and convert text labels into a numerical format.
2. **Model Training:** Train the CRNN model using preprocessed data.
3. **Evaluation:** Evaluate the trained model's performance using evaluation metrics.
4. **Prediction:** Use the trained model to predict text in new handwritten images.

## Dependencies:

- Python (>=3.8)
- TensorFlow
- NumPy
- OpenCV
- Matplotlib
- Pandas

## Repository Structure
- **load_data:** Scripts or classes for loading training and validation images.
- **clean_data:** Scripts for cleaning data, including replacing inappropriate data or deleting.
- **preprocessing:** Scripts for preprocessing data.
- **prepare_dataset:** Scripts for preparing the dataset, including generating output, calculating lengths of dates, and other tasks.
- **model:** Implementation of the CRNN model architecture.
- **data_loader:** Scripts or classes for loading data.
- **training:** Scripts for model training and evaluation.
- **testing:** Scripts for testing the model on validation and test datasets.
- **analysis_and_model_adjustments:** Scripts for analyzing model performance, identifying unrecognized characters, and making adjustments to improve model performance.

## Documentation
- **README.md:** Contains a comprehensive project description, instructions for running, project dependencies, and usage examples.
- **requirements.txt:** List of all project dependencies.

## Start Model
- **start_model.ipynb** Notebook to start model. Each cell should be executed one by one until the end.
- **project_train_model.ipynb** Notebook to train model. 

# Dog Breed Identification using Deep Learning

This is a deep learning project which uses computer vision and transfer learning to classify images of dogs into one of 120 breeds. The model was trained on a dataset of over 10,000 images from a Kaggle competition and uses the MobileNet V2 architecture pretrained on ImageNet.

## Data

The data for this project consists of over 10,000 images of dogs in the training set and over 10,000 images in the test set. Each image is labeled with one of 120 breeds. The dataset is sourced from a Kaggle competition and represents a diverse set of dog breeds.

## Data Preprocessing

The preprocessing steps applied to the images include:
- Reading the image file using TensorFlow and converting it into a tensor.
- Resizing the image to (224, 224) to match the input size for MobileNet V2.
- Normalizing pixel values to be between 0 and 1.

## Model

The model used for this project is MobileNet V2 pre-trained on ImageNet. The base model was combined with a new classifier which was trained on the dog breed dataset.

## Training

The model was trained using the Adam optimizer and Categorical Crossentropy as the loss function. Early stopping was used to prevent overfitting. 

## Evaluation

The evaluation metric used for the competition was Multi-Class Log Loss between the predicted probability and the observed target. My model received a score of 0.88499 which landed on 806 on the leaderboard. 

## Usage

A Google Colab notebook is provided in this repository which includes the complete code for data preprocessing, model training, and evaluation. You can clone this repository and run the notebook to replicate the project or use it as a starting point for your own experiments.

## Contact

For any queries or discussions, feel free to contact me at dakotadurfee23@gmail.com


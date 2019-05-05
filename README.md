# Generate Faces
Face Generation using Pytorch

## Datasets:
This model was trained using the CelebFaces Attribute Dataset (CelebA). 

## Data Processing:
Exploratory analysis, cleaning, normalization, and train/test set splitting were done in the dlnd_face_generation.ipynb notebook. Preprocessing steps included converting to cropping and scaling to 64x64px, and normalizing pixel intensity values between -1 and 1.

## Model Training:
Experiments were conducted using experiments.py and automate.py. Experiments.py created a json file of neural net architectures to be stacked and compiled using ad_lib_model.py. That way, you can queue models to train and let all of them train overnight. Results are logged in results.csv.

## Model Evaluation:
The best performance came from model which had 8 convolutional layers and 1 fully connected layer, achieving a generator loss upto 3.875.

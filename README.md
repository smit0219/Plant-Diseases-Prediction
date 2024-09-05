# Plant-Diseases-Prediction
This project aims to create a machine learning model, specifically a Convolutional Neural Network (CNN), that can classify different types of potato leaf diseases. The data used for training the model comes from the PlantVillage dataset, which contains images of potato leaves affected by different diseases, as well as healthy leaves.
Key Features:

1. Dataset:
The dataset consists of images belonging to three classes:
Potato___Early_blight: A type of fungal infection.
Potato___Late_blight: Another fungal infection, which can be more severe.
Potato___healthy: Images of healthy potato leaves.
There are 2,152 images in total.

2. Image Preprocessing:
Resizing and Rescaling: The images are resized to 256x256 pixels, and their pixel values are scaled to a range between 0 and 1. This standardization helps the model learn more effectively.
Data Augmentation: Techniques like random flipping and rotation are applied to the images during training. This artificially increases the variety of training data, which can improve the model’s ability to generalize to new, unseen images.

3. Data Partitioning:
The dataset is split into three parts:
Training Set (80%): Used to train the model.
Validation Set (10%): Used to tune the model and avoid overfitting.
Test Set (10%): Used to evaluate the model's performance after training.
The code also includes functionality to shuffle the data, ensuring that the training, validation, and test sets are representative of the entire dataset.

4. Performance Optimization:
To speed up the training process, the code includes techniques like caching, shuffling, and prefetching. These steps help the model load and process data more efficiently during training.
Model Architecture:

The CNN model begins with preprocessing layers to resize, rescale, and augment the images. After that, convolutional layers (which detect patterns like edges or textures) will be added to the model (this part of the code is still in progress).
The idea is to create a deep learning model that can automatically learn features from images to classify the type of disease or if the plant is healthy.

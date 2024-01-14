##Celebrity-image-classifier-using-python
Celebrity image classifier using python is a program that automatically identifies celebrities in images. It uses machine  learning and computer vision to analyze and categorize the visual features of the images.

Here's a summary of the key steps:

1. **Preprocessing: Detect face and eyes**
   - Use Haar cascade from OpenCV to detect faces and eyes in the images.
   - Display the detected faces and eyes on the images.

2. **Preprocessing: Crop the facial region of the image**
   - Crop the detected facial region and display the cropped image.

3. **Preprocessing: Use wavelet transform as a feature for training the model**
   - Apply wavelet transform to the cropped image to extract features related to facial features like eyes, nose, and lips.
   - Display the wavelet transformed image.

4. **Preprocessing: Load image, detect face, and save/crop the face region**
   - Define a function that takes an input image, detects faces, and saves/crops the face region only if two eyes are detected.

5. **Dataset Preparation**
   - Go through all images in the dataset folder and create cropped images for them.
   - Manually examine the cropped folder and delete any unwanted images.

6. **Data Cleaning and Preparation**
   - Convert images into suitable formats and prepare X and y for model training.

7. **Model Training**
   - Train a Support Vector Machine (SVM) with an RBF kernel using a pipeline that includes standard scaling.

8. **Model Evaluation**
   - Evaluate the model's performance on the test set and print the classification report.

9. **Model Tuning with GridSearchCV**
   - Try out different models (SVM, Random Forest, Logistic Regression) with different parameters using GridSearchCV to find the best-performing model.

10. **Results**
    - Display the best scores and parameters for each model.

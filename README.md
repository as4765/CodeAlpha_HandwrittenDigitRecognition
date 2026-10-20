# CodeAlpha Task 3: Handwritten Digit Recognition

A Convolutional Neural Network (CNN) that identifies handwritten digits
(0-9), built as part of the CodeAlpha Machine Learning internship.

## Dataset
- MNIST (loaded with Keras)
- 60,000 training images and 10,000 test images
- 28x28 grayscale images, 10 classes (digits 0-9)

## Model Architecture
- Conv2D (32 filters) + MaxPooling
- Conv2D (64 filters) + MaxPooling
- Flatten + Dropout (0.3)
- Dense (128, ReLU)
- Dense (10, Softmax)

## Approach
1. Visualized sample images and class distribution
2. Normalized pixel values (0-1) and reshaped the images for the CNN
3. Trained the model for 8 epochs (Adam optimizer, 10% validation split)
4. Evaluated on the test set with a classification report and confusion
   matrix
5. Inspected correct predictions and misclassified images

## Results
- **Test accuracy: 99.15%**
- About 85 misclassified images out of 10,000
- Most errors happen between similar-looking digits such as 4 and 9  and
  3 and 5

## Future Improvements
- Data augmentation (rotation, shifting)
- Deeper networks
- Extend to letters using EMNIST
- Word recognition with a CRNN

## Tools Used
Python, TensorFlow/Keras, NumPy, scikit-learn, matplotlib, seaborn,
Google Colab

## How to Run
Open `CodeAlpha_HandwrittenDigitRecognition.ipynb` in Google Colab, select
a T4 GPU runtime, and click **Runtime → Run all**.

## Author
Abishek SM
Machine Learning Intern at CodeAlpha

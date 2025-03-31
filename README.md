# Sports Celebrity Image Classification

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify images of sports celebrities.

## Dataset

The dataset used in this project consists of images of four sports celebrities:

-   Cristiano Ronaldo
-   Kobe Bryant
-   Maria Sharapova
-   Kane Williamson

The dataset is divided into training and testing sets.

## Project Structure

-   `Train split/`: Contains the training and validation images.
-   `test split/`: Contains the test images.
-   `main.py`: The Python script that implements the CNN model.

## Dependencies

-   TensorFlow (`tensorflow`)
-   NumPy (`numpy`)
-   scikit-learn (`sklearn`)

You can install these dependencies using pip:

```bash
pip install tensorflow numpy scikit-learn

python main.py

Test accuracy: 1.0
                 precision    recall  f1-score   support

        ronaldo       1.00      1.00      1.00         1
    Kobe Bryant       1.00      1.00      1.00         1
Maria Sharapova       0.00      0.00      0.00         1
Kane Williamson       0.00      0.00      0.00         1

       accuracy                           0.50         4
      macro avg       0.50      0.50      0.50         4
   weighted avg       0.50      0.50      0.50         4

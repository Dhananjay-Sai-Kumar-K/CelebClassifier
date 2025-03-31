# 📸 Sports Celebrity Image Classification 🏆

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify images of sports celebrities. 🧠

## 📁 Dataset

The dataset used in this project consists of images of four sports celebrities:

-   Cristiano Ronaldo ⚽
-   Kobe Bryant 🏀
-   Maria Sharapova 🎾
-   Kane Williamson 🏏

The dataset is divided into training and testing sets. 📂

## 🏗️ Project Structure

Sports-celebrity-image-classification/
├── Train split/
│   ├── ronaldo/
│   ├── Kobe Bryant/
│   ├── Maria Sharapova/
│   └── Kane Williamson/
├── test split/
│   ├── ronaldo/
│   ├── Kobe Bryant/
│   ├── Maria Sharapova/
│   └── Kane Williamson/
└── main.py 🐍

-   `Train split/`: Contains the training and validation images. 🖼️
-   `test split/`: Contains the test images. 🧪
-   `main.py`: The Python script that implements the CNN model. 💻

## 📦 Dependencies

-   TensorFlow (`tensorflow`) ⚡
-   NumPy (`numpy`) 🔢
-   scikit-learn (`sklearn`) 📊

You can install these dependencies using pip:

```bash
pip install tensorflow numpy scikit-learn 🚀

🚀 Usage
Download the Dataset: Download the dataset and place it in the project directory. Ensure the directory structure matches the one described above. 📥
Run the Script: Execute the main.py script:

python main.py 🏃

This script will:

Load the training, validation, and test datasets. 📂
Apply data augmentation to the training dataset. 🔄
Normalize the pixel values. 📈
Define and compile the CNN model. 🧠
Train the model. 🏋️
Evaluate the model on the test dataset. 🧪
Print the test accuracy and classification report. 📊
🧠 Model Architecture
The CNN model architecture used in this project is as follows:

Convolutional layer with 32 filters and a (3, 3) kernel, ReLU activation. 🧱
Max pooling layer with a (2, 2) pool size. ⬇️
Convolutional layer with 64 filters and a (3, 3) kernel, ReLU activation. 🧱
Max pooling layer with a (2, 2) pool size. ⬇️
Convolutional layer with 64 filters and a (3, 3) kernel, ReLU activation. 🧱
Flatten layer. 📉
Dense layer with 64 units, ReLU activation. 🔗
Dense layer with 10 units, softmax activation. 🎯
🔄 Data Augmentation
The following data augmentation techniques are applied to the training dataset:

Random horizontal and vertical flips. ↔️↕️
Random rotations (up to 20 degrees). 🔄
Random zoom (up to 20%). 🔍
Random translations (up to 20% in both height and width). 🗺️
Random contrast adjustments. ☀️🌑
📊 Results
The model achieved the following results on the test dataset:

Test accuracy: 1.0 💯
                 precision    recall  f1-score   support

        ronaldo       1.00      1.00      1.00         1
    Kobe Bryant       1.00      1.00      1.00         1
Maria Sharapova       0.00      0.00      0.00         1
Kane Williamson       0.00      0.00      0.00         1

       accuracy                           0.50         4
      macro avg       0.50      0.50      0.50         4
   weighted avg       0.50      0.50      0.50         4
Note: The test set is very small, consisting of only 4 images. Therefore, the reported accuracy and classification report might not be representative of the model's performance on a larger dataset. The model achieved 100% accuracy on ronaldo and Kobe Bryant test images, but 0% accuracy on the other 2 test images. ⚠️

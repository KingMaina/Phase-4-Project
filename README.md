# Chest-X-Ray-Image_Classification

## Introduction 

This project investigated the use of Deep Learning for classifying chest X-rays into normal and pneumonia cases. We established Convolutional Neural Network (CNN) as the baseline model.

## Business Case

The project aims to detect aid in detectng pneumonia cases quicker. This can be acheived by differentiating healthy lungs from from those infected.
The dataset used is from [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)



## Exploratory Data Analysis


X-ray of a patient with normal lungs:

<img src="........Github........" />

X-ray of a patient with pneumonia:

<img src=".............Github.........." />

- The training images were 1342 for the Normal (healthy) cases and 3876 for Pneumonia cases
- The test images were 234 for the Normal cases and 390 for Pneumonia cases
- Validation Images were 9 for the Normal cases and Pneumonia cases

We also checked for the average image size of the training, testing and validation images. This necessitated the:
    - Resizing
    - Normalizaition
    - Augmentation


## Modeling
### CNN

In the modeling phase, we developed and trained two distinct Convolutional Neural Network (CNN) architectures tailored to our binary image classification task of pneumonia diagnosis from X-ray images. Our first model, the baseline CNN, served as a foundational architecture, while the second model leveraged the ResNet50V2 architecture, known for its depth and performance. Leveraging insights from exploratory data analysis (EDA), we optimized these models for image size, class distribution, and regularization techniques to mitigate overfitting. Through rigorous experimentation and evaluation, we sought to identify the most effective model configurations, utilizing metrics such as accuracy and loss to guide refinement and ensure robust, high-performing classifiers capable of accurately discerning normal from pneumonia cases in X-ray images.

#### CNN Model Performance

- Validation Loss: 30.517587661743164
-Validation Accuracy: 0.5
-Test Loss: 19.448657989501953
-Test Accuracy: 0.625

Validation accuracy of 0.5 wasn't ideal but could be improved by training more on the dataset. In our case we utilized a different cnn architecture.

### ResNet50V2
The results were as follows:

-Validation Loss: 0.2682477533817291
-Validation Accuracy: 0.875
-Test Loss: 0.23323379456996918
-Test Accuracy: 0.9150640964508057

The validation accuracy of 0.87 performed better and ResNet50V2 proved to be better for identify pneumonia.

## Conclusion

## Recommendations





- Get more data for the validation set to gain a better/realistic model accuracy

- Trying/explore different parameters and layers for the neural network modeling

- Create more unique images by augmenting some of given data to give the machine more data to train from

























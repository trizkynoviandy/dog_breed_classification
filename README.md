# Dog Breed Classification

This project aims to develop a deep learning model for dog breed classification using the ResNet50 architecture. The ResNet50 is a pre-trained convolutional neural network (CNN) model that is commonly used in image classification tasks.

## Dataset

The dataset can be downloaded from the [Kaggle](https://www.kaggle.com/datasets/yapwh1208/dogs-breed-dataset).
The dataset consists of 5 common dog's breeds:
* French Bulldog (208 images)
* German Shephard (247 images)
* Golden Retriever (213 images)
* Poodle (182 images)
* Yorkshire Terrier (180 images)

## Methodology

We used transfer learning to fine-tune the ResNet50 model on the dataset. Transfer learning is a technique in deep learning where a pre-trained model is used as a starting point for a new task. By using a pre-trained model, we can reduce the training time and improve the accuracy of the model.

We first initialized the ResNet50 model with pre-trained weights on the ImageNet dataset. We then removed the last layer of the model and replaced it with a new fully connected layer with 120 nodes, corresponding to the number of dog breeds in the dataset. We froze the weights of the pre-trained layers and only trained the new fully connected layer. We used the categorical cross-entropy loss function and the Adam optimizer to train the model.

## Results

After training the model on the training set and evaluating it on the validation set, we achieved an accuracy of 98.29%. We then evaluated the model on the testing set and 
achieved an accuracy of 98.44%.

## Conclusion

In this project, we developed a deep learning model for dog breed classification using the ResNet50 architecture. We achieved an accuracy of 98.44% on the testing set. This model can be used for various applications, such as identifying dog breeds in images and assisting in the development of pet-related apps.


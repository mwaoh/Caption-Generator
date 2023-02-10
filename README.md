# Caption-Generator
Training a Convolutional Neural Network CNN to generate Image Captions

## Process
Step 1: Data Preparation

1. Collect a dataset of images and their corresponding captions.
2. I preprocessed the captions by tokenizing them (i.e., splitting them into individual words) and applying text normalization techniques such as lower-casing and stemming.
3. I created a vocabulary of the most common words in the captions. This vocabulary will be used to create numerical representations of the words in the captions.
4. I converted the captions into numerical sequences by replacing each word with its corresponding index in the vocabulary.
5. I split the dataset into training, validation, and test sets.
6. I created batches of data for training by selecting a batch size and sampling images and their captions from the training set.
7. I preprocessed the images in the batches by applying normalization techniques such as mean subtraction and standardization.
8. I generated captions for the images in the batches by feeding the images through the image encoder part of the model and using the resulting encodings to predict the corresponding captions.
9. I train the model by minimizing the difference between the predicted captions and the ground truth captions.

Step 2: Model

A convolutional neural network (CNN)  to encode the image(A pretrained Resnet50 model) and a recurrent neural network (RNN) to decode the caption. This is because CNNs are good at extracting features from images, and RNNs are good at processing sequences of data such as text

Step 3: Evaluation

The Model performs badly, and we cannot trust the model, because it overfitted, meaning it had an average train and validation loss, but performed very poorly on the test set, the training dataset is quite small for such a task which  also had a  major effect.


About this project.

The project involves building a model that can suggest descriptive captions for images of nature and wildlife. The goal is to increase user engagement on a social platform by providing users with suggestions for captions to use with their images.

As for measurable results, some potential metrics that could be used to evaluate the effectiveness of the model could include:

    The number of users who choose to use the model's caption suggestions
    The increase in engagement (e.g., likes, comments, shares) on posts that use the model's caption suggestions
    User satisfaction with the model's caption suggestions, as measured through surveys or other feedback mechanisms
    The impact of the model's caption suggestions on the overall usage of the platform (e.g., time spent on the platform, number of posts made)

It would be important to establish baseline values for these metrics before deploying the model, and then to track the changes in these metrics over time in order to determine the impact of the model on user engagement.


Outcomes
A model that is able to accurately and consistently suggest descriptive captions for images of nature and wildlife.



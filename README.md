# Image Caption Generation 
 Image Caption Generation on Flickr8K Dataset



# Introduction
Without the deeplearning and AI algorithms, this problem was very different to solve even for computer scientists because normal computers cannot understand the images as humans do. With the aid of Deep learning we can solve this problem easily.

Image caption generator is an interesting task where both computer vision techniques and natural language processing techniques are explored to recognize the context of an image and outline them in a natural language like English.


# Objective

The Objective of our project is to build a working model of image caption generator by using CNN (Conventional Neural networks) with LSTM (Long short term memory), RNN and GRU. In simple words, Our goal is to build a model which takes an image as input and outputs its caption.

# Dataset
We are using Flickr8K dataset for image caption generation available in Kaggle[2].

Flickr8K.zip comprises of two folders:

• Flickr8K_Images: Contains a total of 8000 jpeg images of different shapes and sizes. We are using 6000 images for training, 1000 images for testing and 1000 images for validation

• Flickr8K_TextData: Contains text files describing the images in the train, validation and the test sets. Each image has a total of 5 captions i.e. a total of 40000 captions

The dataset consists of images gathered from different Flickr groups, so the Flickr8K dataset contains a variety of images depicting scenes and situations. The images are currently of different dimensions i.e. 415x502, 500x332, 333x500 etc.


# Results

[![Screen-Shot-2020-12-22-at-9-04-34-PM.png](https://i.postimg.cc/7YtZtyGS/Screen-Shot-2020-12-22-at-9-04-34-PM.png)](https://postimg.cc/ZC3m02Lq)

[![Screen-Shot-2020-12-22-at-9-11-24-PM.png](https://i.postimg.cc/prXPk0P0/Screen-Shot-2020-12-22-at-9-11-24-PM.png)](https://postimg.cc/dkpMVjkd)

[![Screen-Shot-2020-12-22-at-9-11-38-PM.png](https://i.postimg.cc/X7Pnccm8/Screen-Shot-2020-12-22-at-9-11-38-PM.png)](https://postimg.cc/ppDNP82h)

# BLEU Score
Evaluating the Performance using Bilingual Evaluation Understudy Score (BLEU) metric for each model
• BLEU is a metric for evaluating a generated sentence to a reference sentence

• BLEU score lies between 0 and 1, where a perfect match results in a score of 1 and a perfect mismatch results in a score of 0

• It counts the matching n-grams in the generated and the reference description, where 1-gram or unigram would be each token and a bigram comparison would be each word pair

• The n-gram comparison is made regardless of word order

• BLEU ensures that the all the occurrences in the reference text is considered

[![Screen-Shot-2020-12-22-at-9-11-51-PM.png](https://i.postimg.cc/yNmBKqdQ/Screen-Shot-2020-12-22-at-9-11-51-PM.png)](https://postimg.cc/Y4CTNsQY)

# Conclusions¶
We observed that LSTM was performing the best out of all the networks.
The idea of a neural network generating a sentence with proper grammar by looking at an image is utterly fascinating. We were successfully able to generate some good captions, some funny captions and some not so good captions as seen from the results.

The main reason behind the funny captions was due to the model being confused by a predominant presence of a color or object in the image that sidelines the main subject and actions in the image.

This can be fixed using visual attention techniques like soft visual attention or gaussian visual attention that help elevate the importance of the subject and actions in the image.

The descriptions that we generated were very small in terms of length and we attribute this to the limited amount of data that we had for training.

Generally generative models require huge amounts of data during training to be more efficient just like any other neural network.

# References

1) https://arxiv.org/abs/1708.02043
2) https://machinelearningmastery.com/develop-a-deep-learning-caption-generation-model-in-python/
3) https://thinkautonomous.medium.com/rnns-in-computer-vision-image-captioning-597d5e1321d1
4) https://machinelearningmastery.com/calculate-bleu-score-for-text-python/

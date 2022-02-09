# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Neural Networks Image Classification with Fashion MNIST 👗👔

## Goal 

In this lab you will create several neural network models to classify clothing images. Your goal is to obtain the the highest scoring model on the test set with no data leakage.

## Instructions

In a notebook, prepare your data, create and train your model, and evaluate it with a validation split. The training data is [fashion-mnist_train.csv](https://www.kaggle.com/zalando-research/fashionmnist?select=fashion-mnist_train.csv).

- Use Tensorflow Keras.
- Don't forget to use a GPU Accelerator to speed up your training! You may want to use Colab or Kaggle - both have free GPUs - make sure you turn them on. 🚀
- There are many model architectures and hyperparameters you can tune. See what gives you the best validation score.
$$
Then create predictions for the [test set](https://www.kaggle.com/zalando-research/fashionmnist?select=fashion-mnist_test.csv). The predictions should be numbers in the range 0-9. DROP THE LABEL COLUMN FIRST! ⚠

- Do NOT use other people's Kaggle Kernels.

- Visualize each of the image classes.
- Create a simple feed forward model that trains fast.
- Create a confusion matrix to see how your model performs on different articles of clothing.
- Make at least one CNN model. 
 
## Bonus: use data augmentation and/or transfer learning to make a better model.


### The dataset
From Kaggle:

> Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes. Zalando intends Fashion-MNIST to serve as a direct drop-in replacement for the original MNIST dataset for benchmarking machine learning algorithms. It shares the same image size and structure of training and testing splits.

> The original MNIST dataset contains a lot of handwritten digits. Members of the AI/ML/Data Science community love this dataset and use it as a benchmark to validate their algorithms. In fact, MNIST is often the first dataset researchers try. "If it doesn't work on MNIST, it won't work at all", they said. "Well, if it does work on MNIST, it may still fail on others."

Fashion-MNIST dataset on Kaggle: https://www.kaggle.com/zalando-research/fashionmnist


## Have fun and good luck! 🚀

Created by Jeff Hale, adapted from Caroline Schmitt.
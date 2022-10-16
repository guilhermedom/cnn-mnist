# CNN Classifying Images with Handwritten Digits from MNIST

A quick analysis of simple [convolutional neural network] (CNN) architectures classifying images with handwritten digits from the [MNIST dataset].

---

## Problem Overview

Handwritten digits recognition is a long-time popular classification task in machine learning. Its popularity come from the simplicity of the task, useful for testing prototype models, and from being used to test the [first LeNet CNN architectures proposed]. The objective on this task is to build a model that can read any image with a handwritten digit and identify what digit is in the image. The most commonly used dataset for the task has thousands of images in 28x28 resolution, composing a dataset called MNIST. The images belong to 10 classes corresponding to each one of the 10 numerical digits:

![mnist_handwritten](https://user-images.githubusercontent.com/33037020/196017340-7c0d9f52-a02c-4232-97b9-195a7936436e.png)

Many models have been experimented with the MNIST handwritten dataset, including [random forests], [neural networks], [K-Nearest Neighbors] and others. Many different CNN architectures have been proposed to deal with the task and most of them achieved very good results. Some of the proposed models are quite complex and this leads to the question: do we really need complex CNNs to deal with this task?

## Analysis Introduction

CNNs are known to achieve great results when dealing with images, especially because of their convolutional layers which work as good, and rather simple, feature extractors. Even shallow CNNs are able to achieve a great performance while being simple and cheap to train. In this analysis, we show that a simple CNN architecture can be used to get optimal results on MNIST.

Other than that, we also test 4 different variations of our original simple CNN architecture. With this testbed we are able to discuss the effects that each small change impose on model performance. We are able to show that with this shallow architecture, it is possible to achieve above 99% accuracy. It is also possible to get near 99% accuracy with unoptimal choices for number of feature maps or convolutional filter sizes.

Bear in mind that this repository uses a notebook created using TensorFlow-v1 API. Although deprecated, TensorFlow-v1 is still used in many legacy models and is still very functional. This analysis can be used as reference by anyone learning TensorFlow-v1 to understand and maintain old models.

[//]: #

[first LeNet CNN architectures proposed]: <http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf>
[MNIST dataset]: <https://www.kaggle.com/competitions/digit-recognizer/data>
[convolutional neural network]: <https://www.ibm.com/cloud/learn/convolutional-neural-networks>
[random forests]: <https://link.springer.com/article/10.1023/A:1010933404324>
[neural networks]: <https://d2l.ai/chapter_linear-regression/index.html>
[K-Nearest Neighbors]: <https://www.ibm.com/topics/knn>

# Day 5

For day 5, I followed the first coding tutorial of FlowerLabs. The tutorial is really well made!

<img width="217" align="left" alt="Screenshot 2024-11-28 at 20 22 24" src="https://github.com/user-attachments/assets/6fdcd045-f592-4812-8414-06eff2a265cc">


Here's what they cover:

The tutorial begins by guiding you through the process of setting up a centralized training pipeline using PyTorch. This involves defining a simple convolutional neural network (CNN) and training it on the CIFAR-10 dataset. The CIFAR-10 dataset consists of images categorized into ten classes: 'airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', and 'truck'. The tutorial provides detailed instructions on loading and preprocessing the data, defining the CNN architecture, and implementing training and evaluation functions.

After establishing the centralized training setup, the tutorial transitions into federated learning using the Flower framework. It demonstrates how to simulate a federated learning environment by partitioning the CIFAR-10 dataset into multiple subsets, each representing a client in the federated system. The Flower framework is then utilized to coordinate the training process across these simulated clients, aggregating their updates to train a global model.

Throughout the tutorial, key concepts of federated learning are explained, and practical code examples are provided to illustrate the implementation. By the end, you will have a solid understanding of how to set up both centralized and federated learning experiments using PyTorch and the Flower framework.

For more detailed information and access to the code examples, you can refer to the official tutorial on the Flower website.

source: https://flower.ai/docs/framework/tutorial-series-get-started-with-flower-pytorch.html

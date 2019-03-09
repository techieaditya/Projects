# Name: Aditya Prakash
# Email : aditya211p@gmail.com
# Batch : 2.
 ___
 
 ## 1. Convolution 
 ---
 ![Conlvolution](https://www.researchgate.net/profile/Anupama_Ray/publication/274255563/figure/fig2/AS:294965436534787@1447336648880/Block-Diagram-of-Convolutional-Deep-Neural-Network.png)
 

 
### Convolution:
  A convolutional neural network (CNN) is a type of artificial neural network used in image recognition and processing that is specifically designed to process pixel data.

 CNNs are powerful image processing, artificial intelligence (AI) that use deep learning to perform both generative and descriptive tasks, often using machine vison that includes image and video recognition, along with recommender systems and natural language processing (NLP).

   A neural network is a system of hardware and/or software patterned after the operation of neurons in the human brain. Traditional neural networks are not ideal for image processing and must be fed images in reduced-resolution pieces. CNN have their “neurons” arranged more like those of the frontal lobe, the area responsible for processing visual stimuli in humans and other animals. The layers of neurons are arranged in such a way as to cover the entire visual field avoiding the piecemeal image processing problem of traditional neural networks.

## 2. Filters/Kernels:
---
![](https://www.researchgate.net/profile/Haidar_Khan/publication/322058908/figure/fig2/AS:650790163202050@1532171874975/CNN-architecture-Convolutional-layers-learn-a-set-of-filters-kernels-that-are-convolved.png)

### Filters/Kernels :
   The filter is a well defined operation for any set of parameters (convolution kernel) or input data we can think of.
We can draw a following connection between the linear filter and the convolutional neural network:

![Kernels](https://cdn-images-1.medium.com/max/800/1*Dib0PZFF5kz3jlQMC2nv1Q.png)

The learning task can now be stated as a minimization problem where the mean squared error between the output of the linear filter and the output of the convolutional neural network is minimized:
 ## 3 . 1x1 Convolution :
 ---
 ![Convolution](https://raw.githubusercontent.com/iamaaditya/iamaaditya.github.io/master/images/conv_arithmetic/full_padding_no_strides_transposed_small.gif)
### 1x1 convolution : 
One by One convolution was first introduced in this paper titled Network in Network. In this paper, the author’s goal was to generate a deeper network without simply stacking more layers. It replaces few filters with a smaller perceptron layer with mixture of 1x1 and 3x3 convolutions. In a way, it can be seen as “going wide” instead of “deep”, but it should be noted that in machine learning terminology, ‘going wide’ is often meant as adding more data to the training. Combination of 1x1 (x F) convolution is mathematically equivalent to a multi-layer perceptron.

## 4. Epochs :
 ---
### Epoch :
   In Deep Learning, an epoch is a hyperparameter which is defined before training a model. One epoch is when an entire dataset is passed both forward and backward through the neural network only once.

   
   One epoch is too big to feed to the computer at once. So, we divide it in several smaller batches. We use more than one epoch because passing the entire dataset through a neural network is not enough and we need to pass the full dataset multiple times to the same neural network. But since we are using a limited dataset and to optimise the learning and the graph we are using Gradient Descent which is an iterative process. So, updating the weights with single pass or one epoch is not enough.In training neural network, one epoch means one pass of the full training set. Usually it may contain a few iterations.
    Because usually we divide the training set into batches, each epoch go through the whole training set. Each iteration goes through on batch
    
## 5. Feature Maps :
   The feature map is the output of one filter applied to the previous layer. A given filter is drawn across the entire previous layer, moved one pixel at a time. Each position results in an activation of the neuron and the output is collected in the feature map. You can see that if the receptive field is moved one pixel from activation to activation, then the field will overlap with the previous activation by (field width - 1) input values.
For instance, In a 32 × 32 image , dragging the 5 × 5 receptive field across the input image data with a stride width of 1 will result in a feature map of 28 × 28 (32–5+1 × 32–5+1) output values or 784 distinct activations per image. Think of it as representations of the input. The number of filters (kernel) you will use on the input will result in same amount of feature maps. Think of filter like a membrane that allows only the desired qualities of the input to pass through it.
    ![Feature Map](https://qph.fs.quoracdn.net/main-qimg-134024e4e35d7c7cbc4ccbe3a62dc8b2.webp)
    
 

### RESNET50
ResNet50 is a deep convolutional neural network (CNN) architecture that was developed by Microsoft Research in 2015. It is a variant of the popular ResNet architecture, which stands for “Residual Network.” The “50” in the name refers to the number of layers in the network, which is 50 layers deep.

ResNet50 is a powerful image classification model that can be trained on large datasets and achieve state-of-the-art results. One of its key innovations is the use of residual connections, which allow the network to learn a set of residual functions that map the input to the desired output. These residual connections enable the network to learn much deeper architectures than was previously possible, without suffering from the problem of vanishing gradients.

### ARCHITECTURE OVERVIEW

![image](https://github.com/Ro-han12/CAEI_AI_MODELS/assets/95674406/1858b0ce-0778-45ae-a392-0a2a4a8e7923)

The architecture of ResNet50 is divided into four main parts: the convolutional layers, the identity block, the convolutional block, and the fully connected layers. The convolutional layers are responsible for extracting features from the input image, while the identity block and convolutional block are responsible for processing and transforming these features. Finally, the fully connected layers are used to make the final classification.

The convolutional layers in ResNet50 consist of several convolutional layers followed by batch normalization and ReLU activation. These layers are responsible for extracting features from the input image, such as edges, textures, and shapes. The convolutional layers are followed by max pooling layers, which reduce the spatial dimensions of the feature maps while preserving the most important features.

The identity block and convolutional block are the key building blocks of ResNet50. The identity block is a simple block that passes the input through a series of convolutional layers and adds the input back to the output. This allows the network to learn residual functions that map the input to the desired output. The convolutional block is similar to the identity block, but with the addition of a 1x1 convolutional layer that is used to reduce the number of filters before the 3x3 convolutional layer.

The final part of ResNet50 is the fully connected layers. These layers are responsible for making the final classification. The output of the final fully connected layer is fed into a softmax activation function to produce the final class probabilities.

### VERSIONS
1.ResNet50 function
keras.applications.ResNet50(
    include_top=True,
    weights="imagenet",
    input_tensor=None,
    input_shape=None,
    pooling=None,
    classes=1000,
    classifier_activation="softmax",
)
2.ResNet101 function
keras.applications.ResNet101(
    include_top=True,
    weights="imagenet",
    input_tensor=None,
    input_shape=None,
    pooling=None,
    classes=1000,
    classifier_activation="softmax",
)
3.ResNet152 function
keras.applications.ResNet152(
    include_top=True,
    weights="imagenet",
    input_tensor=None,
    input_shape=None,
    pooling=None,
    classes=1000,
    classifier_activation="softmax",
)
4.ResNet50V2 function
keras.applications.ResNet50V2(
    include_top=True,
    weights="imagenet",
    input_tensor=None,
    input_shape=None,
    pooling=None,
    classes=1000,
    classifier_activation="softmax",
)
5.ResNet101V2 function
keras.applications.ResNet101V2(
    include_top=True,
    weights="imagenet",
    input_tensor=None,
    input_shape=None,
    pooling=None,
    classes=1000,
    classifier_activation="softmax",
)
6.ResNet152V2 function
keras.applications.ResNet152V2(
    include_top=True,
    weights="imagenet",
    input_tensor=None,
    input_shape=None,
    pooling=None,
    classes=1000,
    classifier_activation="softmax",
)

### Arguments
1.include_top: whether to include the fully-connected layer at the top of the network.
2.weights: one of None (random initialization), "imagenet" (pre-training on ImageNet), or the path to the weights file to be loaded.
3.input_tensor: optional Keras tensor (i.e. output of layers.Input()) to use as image input for the model.
input_shape: optional shape tuple, only to be specified if include_top is False (otherwise the input shape has to be (224, 224, 3) (with "channels_last" data format) or (3, 224, 224) (with "channels_first" data format). It should have exactly 3 inputs channels, and width and height should be no smaller than 32. E.g. (200, 200, 3) would be one valid value.
4.pooling: Optional pooling mode for feature extraction when include_top is False.
None means that the output of the model will be the 4D tensor output of the last convolutional block.
avg means that global average pooling will be applied to the output of the last convolutional block, and thus the output of the model will be a 2D tensor.
max means that global max pooling will be applied.
5.classes: optional number of classes to classify images into, only to be specified if include_top is True, and if no weights argument is specified.
6.classifier_activation: A str or callable. The activation function to use on the "top" layer. Ignored unless include_top=True. Set classifier_activation=None to return the logits of the "top" layer. When loading pretrained weights, classifier_activation can only be None or "softmax".

### Summary of ResNet:

ResNet, short for Residual Network, is a deep convolutional neural network (CNN) architecture developed by Microsoft Research in 2015. It is designed to address the problem of vanishing gradients in deep neural networks by introducing residual connections. The key innovation of ResNet is the use of residual blocks, which allow the network to learn residual functions that map the input to the desired output. This enables the training of much deeper networks (e.g., ResNet50, ResNet101, ResNet152) without suffering from degradation in performance.

### Uses of ResNet:

1. **Image Classification**: ResNet is commonly used for image classification tasks, where it can achieve state-of-the-art results on large-scale datasets like ImageNet.

2. **Object Detection**: ResNet features are often used as a backbone in object detection systems, such as Faster R-CNN and Mask R-CNN, to extract features from input images.

3. **Semantic Segmentation**: ResNet can be employed in semantic segmentation tasks to classify each pixel in an image into predefined categories.

4. **Transfer Learning**: Pretrained versions of ResNet on datasets like ImageNet are widely used for transfer learning. By fine-tuning these pretrained models on specific datasets, users can achieve good performance on custom tasks with less data.

### Advantages of ResNet:

1. **Deep Architectures**: ResNet enables the training of very deep neural networks with hundreds of layers, leading to improved performance on various computer vision tasks.

2. **Vanishing Gradient Problem**: Residual connections mitigate the vanishing gradient problem, allowing gradients to flow more easily during training. This enables the training of deeper networks without degradation in performance.

3. **State-of-the-Art Performance**: ResNet architectures consistently achieve state-of-the-art results on benchmark datasets for image classification and related tasks.

4. **Transfer Learning**: Pretrained ResNet models can be used for transfer learning, providing a powerful starting point for new computer vision tasks with limited data.

### Disadvantages of ResNet:

1. **Increased Computational Complexity**: Deeper architectures like ResNet require more computational resources for training and inference compared to shallower networks.

2. **Overfitting**: Although residual connections help mitigate the vanishing gradient problem, they may also increase the risk of overfitting, especially when training on small datasets.

3. **Memory Consumption**: ResNet's deep architectures may consume a significant amount of memory, especially when training on large-scale datasets, leading to higher memory requirements for GPUs.

4. **Complexity and Interpretability**: Deeper networks are often more difficult to interpret and analyze compared to shallower architectures, making it challenging to understand the internal representations learned by the model.

Despite these limitations, ResNet remains one of the most widely used architectures in the field of computer vision, demonstrating its effectiveness and versatility in various applications.
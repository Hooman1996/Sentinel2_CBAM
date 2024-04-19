# Sentinel2_CBAM
Unofficial implementation of the paper "A new attention-based CNN approach for crop mapping using time series Sentinel-2 images"

This project implements a deep learning model for crop-type classification using Sentinel-2 satellite images. The model is built with TensorFlow Keras and incorporates advanced architectural components such as Convolutional Block Attention Modules (CBAM) and Residual Units.

**Convolutional Block Attention Module (CBAM)**: CBAM is a type of attention mechanism that can be integrated into any CNN architecture seamlessly. CBAM computes attention maps along two separate dimensions, channel and spatial, then performs feature refinement accordingly. This allows the model to focus on more informative features for the task of crop type classification.
Here You can see the Architectures of CBAM and its sub-modules: (a) CBAM; (b) channel attention module; (c)
![image](https://github.com/Hooman1996/Sentinel2_CBAM/assets/67710406/99ac6c7a-8949-42e3-bac7-26f151c23dcc)

**Residual Units**: The model also uses Residual Units and ResBlocks, a key component of ResNet architecture, which allows the training of deeper networks by providing shortcut connections that bypass convolutional layers. These connections mitigate the problem of vanishing gradients, enabling the model to learn more complex representations.

**Crop Type Classification**: The model is trained and evaluated on Sentinel-2 satellite images. Sentinel-2 provides high-resolution multispectral images, which are ideal for crop-type classification tasks. The model predicts the type of crop present in a given image patch, which can be useful for agricultural planning and monitoring.

The implementation includes data preprocessing, model training, and evaluation steps. Preprocessing involves normalizing the images and splitting the dataset into training, validation, and test sets. The model is trained using a suitable loss function and optimizer, and its performance is evaluated based on accuracy and other relevant metrics on the test set.

Please refer to the individual scripts and notebooks in this repository for more detailed information about each step of the process.
```


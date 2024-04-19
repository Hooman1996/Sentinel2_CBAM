# Sentinel2_CBAM
Unofficial implementation of the paper "A new attention-based CNN approach for crop mapping using time series Sentinel-2 images"
Shout out to the authors for their work.
This project implements a deep learning model for crop-type classification using Sentinel-2 satellite images. The model is built with TensorFlow Keras and incorporates advanced architectural components such as Convolutional Block Attention Modules (CBAM) and Residual Units.

**Convolutional Block Attention Module (CBAM)**: CBAM is a type of attention mechanism that can be integrated into any CNN architecture seamlessly. CBAM computes attention maps along two separate dimensions, channel and spatial, then performs feature refinement accordingly. This allows the model to focus on more informative features for the task of crop type classification.
Here You can see the Architectures of CBAM and its sub-modules: (a) CBAM; (b) channel attention module; (c)
![image](https://github.com/Hooman1996/Sentinel2_CBAM/assets/67710406/99ac6c7a-8949-42e3-bac7-26f151c23dcc)

**Residual Units**: The model also uses Residual Units and ResBlocks, a key component of ResNet architecture, which allows the training of deeper networks by providing shortcut connections that bypass convolutional layers. These connections mitigate the problem of vanishing gradients, enabling the model to learn more complex representations.

**Crop Type Classification**: The model is trained and evaluated on Sentinel-2 satellite image time series. Sentinel-2 provides high-resolution multispectral images, which are ideal for crop-type classification tasks. The model predicts the type of crop present in a given image patch, which can be useful for agricultural planning and monitoring. In this paper 36 images each with 10 bands are used as the input data and the output is the crop type probabilities of 5 different crop types.
Here You can see the full architecture of the implemented model:
![image](https://github.com/Hooman1996/Sentinel2_CBAM/assets/67710406/00f4bb55-94d1-4be1-a075-9706dc6f298e)

Please refer to the original paper for more detailed information about each step of the process.
DOI:  https://www.sciencedirect.com/science/article/pii/S0168169921001083
```


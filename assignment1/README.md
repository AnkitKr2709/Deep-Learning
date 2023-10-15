# Deep-Learning for Image Super-Resolution: A Survey

Image Super-Resolution (SR) is a vital image processing technique, revolutionized by deep learning, that enhances image and video resolution in computer vision. This repository presents a comprehensive survey of recent deep learning-driven SR advancements. The research paper classifies these studies into three key categories: supervised SR, unsupervised SR, and domain-specific SR. Furthermore, as part of this work, we've implemented several supervised SR algorithms using TensorFlow on the 'tf_flowers' dataset. This dataset employs low-resolution images as inputs, and the resulting super-resolution images are compared against the original high-resolution images to demonstrate the efficacy of these techniques.

[**Research Paper**](https://arxiv.org/pdf/1902.06068v2.pdf)

## Implementation

We have implemented the following 3 methods for image super resolution in this repository.:
1. SRCNN [1]
2. FSRCNN 
3. SRGAN [2]

##  Super-Resolution Convolutional Neural Network (SRCNN)

**Model Architecture**

![screenshot_1](Screenshots\s1.jpg)

**Upsampling Method used**: Bicubic Interpolation.

**Framework used**: Pre-upsampling SR

**Loss Function used**: MSE

**Output**:

![screenshot_2](Screenshots\s2.png)


##  Fast Super-Resolution Convolutional Neural Network (FSRCNN)

**Model Architecture**

![screenshot_3](Screenshots\s3.png)

**Upsampling Method used**: Deconv.

**Framework used**: Post-upsampling SR

**Loss Function used**: MSE

**Output**:

![screenshot_4](Screenshots\s4.png)


##  Super Resolution Generative Adversarial Networks (SRGAN)

**Model Architecture**

![screenshot_5](Screenshots\s4.1.png)

**Upsampling Method used**: Sub-pixel convolutional layer.

**Framework used**: Post-upsampling SR

**Loss Function used**: Adversarial loss and a Content loss.

**Output**:

![screenshot_6](Screenshots\s5.png)
![screenshot_7](Screenshots\s6.png)



## References

[1] Learning a deep convolutional network for image super-resolution using SRCNN  [Reseach paper](https://medium.com/analytics-vidhya/srcnn-paper-summary-implementation-ad5cea22a90e)

[2] Super resolution GAN (SRGAN) in keras  [Video link](https://www.youtube.com/watch?v=1HqjPqNglPc&t=643s)
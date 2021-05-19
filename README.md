# Image Style Transfer
Deep Learning, ECE-GY 9123
NYU Spring 2021
cwc478, kyh275

## Introduction
We want to build an image-to-image translation model that maps the style of an image to another domain image while retaining the structure. *Domain* implies a visually distinctive category, and style is a unique appearance of each image. For example, the image-to-image translation transfers the pattern of cheetah to a dog image.

## Model and Dataset
Our model bases on [StarGAN v2](https://github.com/clovaai/stargan-v2).   And, we train it with three datasets: [Animal Faces-HQ (AFHQ)](https://github.com/clovaai/stargan-v2), [CelebFaces Attributes (CelebA)](https://github.com/clovaai/stargan-v2), [Architectural Style](https://sites.google.com/site/zhexuutssjtu/projects/arch).

## Result
We train our model on Amazon SageMaker with 4vCPU, 1 GPU. The iteration is set to 100K for our results.

AFHQ:
![AFHQ](https://github.com/1018WeiChihCheng/DeepLearning/blob/main/ref_0100000.jpg?raw=true)

CelebA:
![CelebA](https://github.com/1018WeiChihCheng/DeepLearning/blob/main/cel_ref_0100000.jpg?raw=true)

Architectural Style:
![Architectural Style](https://github.com/1018WeiChihCheng/DeepLearning/blob/main/a_ref_0100000.jpg?raw=true)
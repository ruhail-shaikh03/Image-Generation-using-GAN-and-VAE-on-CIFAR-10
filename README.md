# Image Generation using GAN and VAE on CIFAR-10 (Cats & Dogs)

This project implements and compares two generative models, a Generative Adversarial Network (GAN) with a custom similarity-based discriminator and a Variational Autoencoder (VAE), for generating images of cats and dogs from the CIFAR-10 dataset.

## Objectives

*   Implement a custom GAN where:
    *   The **Generator** follows an architecture suitable for image generation (e.g., based on DCGAN principles discussed in class).
    *   The **Discriminator** is a custom neural network that evaluates the **similarity** between two images (one real, one generated) and outputs a similarity score.
        *   The Discriminator aims to maximize the dissimilarity score between real and generated images.
        *   The Generator aims to minimize this dissimilarity score, producing more realistic outputs.
*   Implement one or more **diversity-promoting techniques** during GAN training (e.g., Mini-Batch Discrimination, Feature Matching) to avoid mode collapse.
*   Implement a **Variational Autoencoder (VAE)** for the same image generation task.
*   Train both models using only the **"cat" and "dog" classes** from the CIFAR-10 dataset.
*   Compare the GAN and VAE based on:
    *   Visual quality of generated images.
    *   Convergence behavior during training.
    *   Suitable quantitative metrics (e.g., reconstruction loss for VAE, similarity score for GAN, FID/IS if feasible).

## Dataset

*   **CIFAR-10 Dataset:** Consists of 60,000 32x32 color images in 10 classes.
    *   **URL:** [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html)
*   For this project, the dataset is **filtered to include only the "cat" and "dog" classes**.
*   Images are 32x32 pixels with 3 color channels.

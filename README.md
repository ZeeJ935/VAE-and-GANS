# Variational Autoencoders (VAE) & Generative Adversarial Networks (GANs)

This repository contains implementations of Variational Autoencoders (VAEs) and Generative Adversarial Networks (GANs) applied to MNIST numbers, MNIST fashion, and pneumonia anomaly detection using Chest X-ray images.

## Project Overview
We implemented five different models:
1. **GAN for MNIST Numbers**
2. **GAN for MNIST Fashion**
3. **VAE for MNIST Numbers**
4. **VAE for MNIST Fashion**
5. **VAE for Pneumonia Anomaly Detection (Chest X-ray Classification: Normal vs. Pneumonia)**

## Dataset
- **MNIST Numbers & Fashion:** Downloaded from torchvision datasets.
- **Chest X-ray Dataset:** Used for pneumonia classification, preprocessed and stored in the appropriate directories.

## Model Implementations
### 1. GANs
- **Architecture:** A generator and a discriminator trained adversarially.
- **Loss Function:** Binary Cross-Entropy (BCE) loss.
- **Training Strategy:**
  - The generator learns to create realistic images.
  - The discriminator distinguishes between real and generated images.
- **Evaluation:** Generate images and visualize training performance.

### 2. VAEs
- **Architecture:** Encoder, latent space, and decoder.
- **Loss Function:** Combination of Reconstruction Loss (MSE) and KL Divergence.
- **Latent Space Manipulation:** Used for feature extraction and image synthesis.
- **Applications:**
  - MNIST reconstructions.
  - Pneumonia classification using latent space features with PCA.

## Results
- GANs: Generated images from MNIST and Fashion datasets.
- VAEs: Reconstructed images and visualized latent space representations.
- Pneumonia Detection: Classified normal vs. pneumonia cases using VAE and PCA.

# Painting Style Transfer: Project Overview
- Built a CycleGAN to transfer the painting style of Claude Monet onto landscape images. Custom autoencoder architectures were implemented, additional loss functions were tested, and various optimizers were experimented with in order to distill interesting, fun results.
- GAN, or Generative Adversarial Network, is a neural network strategy for generating images. It consists of training two neural network models: a generator and a discriminator. The Generator which is trained to generate images which fit some criteria. The Discriminator is trained to evaluate the output of the Generator model on staying accurate to the criteria.
- CycleGAN is a type of GAN that couples two GANs together – two Generator networks, and two Discriminator networks. The purpose of this GAN architecture is to capture the style and texture of many images, and successfully commit Style Transfer to multiple target images, without needing image pairs. Further details under Section 1.3 of ProjectPaper.pdf.

# Approach
1. Monet and landscape image data is loaded, analyzed, and preprocessed (resizing and optionally normalized to create consistent inputs for our Neural Network)
2. Model Building Blocks are established (Generator & Discriminator Network architecture creation and weight initialization function instantiation) ![PHOTO-2023-12-05-11-32-40](https://github.com/adhr1t/Painting_Style_Transfer/assets/72672768/7c6a6af8-240d-41f7-bb69-ef6ee6d72b32)

3. CycleGAN architecture is built
4. CycleGAN training (loss functions over time visualized to ensure proper training)
5. Hyperparameter Tuning
6. Alternative Loss and Optimizer functions
7. Final Results and Analysis

# Outputs



# Painting Style Transfer: Project Overview
- Built a CycleGAN to transfer the painting style of Claude Monet onto landscape images. Custom autoencoder architectures were implemented, additional loss functions were tested, and various optimizers were experimented with in order to distill interesting, fun results.
- GAN, or Generative Adversarial Network, is a neural network strategy for generating images. It consists of training two neural network models: a generator and a discriminator. The Generator which is trained to generate images which fit some criteria. The Discriminator is trained to evaluate the output of the Generator model on staying accurate to the criteria.
- CycleGAN is a type of GAN that couples two GANs together – two Generator networks, and two Discriminator networks. The purpose of this GAN architecture is to capture the style and texture of many images, and successfully commit Style Transfer to multiple target images, without needing image pairs. Further details under Section 1.3 of ProjectPaper.pdf.

# Approach
1. Monet and landscape image data is loaded, analyzed, and preprocessed (resizing and optionally normalized to create consistent inputs for our Neural Network)
2. Model Building Blocks are established (Generator & Discriminator Network architecture and weight initialization function) 

  *Generator Architecture*:

  ![PHOTO-2023-12-05-11-32-40](https://github.com/adhr1t/Painting_Style_Transfer/assets/72672768/7c6a6af8-240d-41f7-bb69-ef6ee6d72b32) 

3. CycleGAN architecture is built
4. CycleGAN training (loss functions over time visualized to ensure proper training)
5. Hyperparameter Tuning
6. Alternative Loss and Optimizer functions (RMSProp, SGD, AdaGrad, Adam)
7. Final Results and Analysis

# Outputs
A look at some of the outputs produced.

![adagrad_output](https://github.com/adhr1t/Painting_Style_Transfer/assets/72672768/b17c5fa8-cace-46cb-addf-9dacfce7e919)
![basic_Gen_basic_Desc_output](https://github.com/adhr1t/Painting_Style_Transfer/assets/72672768/853b41b1-7eb7-47b1-8201-1f9f9895290d)
![new_G_new_D_output](https://github.com/adhr1t/Painting_Style_Transfer/assets/72672768/ea7bebc7-2484-4406-89c4-371226fc5489)

Not too shabby !

# Conclusion
Generative AI is something that is deeply interesting to me because it has such an important practical application to the ever changing landscape of Machine Learning. Whether it be image data augmentation, text-to-image generation, or transfering your favorite artist's painting style onto standard images, Generative AI is extremely interesting and has exponentially growing applications. I have learned a huge amount throughout the course of this project and I am very satisified with the results this CycleGAN was able to produce. It's definitely a better painter than me !



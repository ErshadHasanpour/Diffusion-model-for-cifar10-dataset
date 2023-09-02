# Diffusion-model-for-cifar10-dataset

In this code, a well known dataset,‘cifar10’, with 32x32 square images from 10 classes has been used to implement the idea of diffusion models on them. For the forward step, we used the reparameterization trick to add noise on original image as a function of time steps. Indicated below is the original image and noisy images in time steps 20, 40, 60 and 80.
![Diff_cifar10_1](https://github.com/ErshadHasanpour/Diffusion-model-for-cifar10-dataset/assets/96794427/34f3095a-6e0f-44a6-a2e3-dbd890cf7148)

After which a modified U-net, with additional self-attention layers, was applied to be trained upon these images in consequent time steps. Due to lack of ultra-fast processors the corresponding U-net was trained for only 20 epochs. Finally, when our U-net was trained we employed it to the Annealed Langevin dynamics algorithm to generate some new images, which 10 of them are illustrated below. 
![Diff_cifar10_2](https://github.com/ErshadHasanpour/Diffusion-model-for-cifar10-dataset/assets/96794427/c3c4d738-a82b-40b1-9476-300fd41f77f8)

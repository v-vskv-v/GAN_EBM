# Improving GAN inference with EBM model

This repository contains code for Final Project of ML Course in Skoltech with experiment results:
- `moons`/`roll`: experiment plots for GAN and proposed model;
- `mnist`/`cifar10`: generated images by GAN and proposed model at each 1000 step;
- `Presentation_GAN_EBM.pdf`: project presentation;
- `Project_GAN_EBM.ipynb`: notebook with code and experiment results;

To run this code and reproduce results you need install these packages and libraries, you have to use `python3.8`. Please, set up a virtual environment and use `pip install -r requirements.txt`.

Below you can find the best results in experiments.

## Moons
An experiment with vanilla GAN, comparison between true distribution and generator distribution.
![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/moons/GAN.png)

An experiment with proposed model, comparison between true distribution and 60 steps of MCMC applied to generator output with step size 3.
![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/moons/GAN_EBM.png)

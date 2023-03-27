# Improving GAN inference with EBM model

This repository contains code for Final Project of ML Course in Skoltech with experiment results:
- `moons`/`roll`: experiment plots for GAN and proposed model;
- `mnist`/`cifar10`: generated images by GAN and proposed model at each 1000 step;
- `Presentation_GAN_EBM.pdf`: project presentation;
- `Report_GAN_EBM.pdf`: project report;
- `Project_GAN_EBM.ipynb`: notebook with code and experiment results;

To run this code and reproduce results you need install these packages and libraries, you should use `python3.8`. Please, set up a virtual environment and use `pip install -r requirements.txt`.

Below you can find the best results in experiments.

## Moons
An experiment with vanilla GAN, comparison between true distribution and generator distribution.
![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/moons/GAN.png)

An experiment with proposed model, comparison between true distribution and 1500 steps of MCMC applied to generator output with step size 2.
![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/moons/GAN_EBM.png)

## Swiss roll
An experiment with vanilla GAN, comparison between true distribution and generator distribution.
![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/roll/GAN.png)

An experiment with proposed model, comparison between true distribution and 1500 steps of MCMC applied to generator output with step size 3.
![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/roll/GAN_EBM.png)

## MNIST
Comparison between generated images by vanilla GAN generator and 500 steps of MCMC  applied to generator output with step size 2.

Images by GAN generator.

![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN/step38000.jpg "Vanilla GAN") ![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN/step35000.jpg "Vanilla GAN") ![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN/step30000.jpg "Vanilla GAN") ![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN/step36000.jpg "Vanilla GAN")

Images by proposed generative model.

![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN_EBM/step11000.jpg "Proposed model") ![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN_EBM/step10000.jpg "Proposed model") ![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN_EBM/step8000.jpg "Proposed model") ![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/mnist/GAN_EBM/step12000.jpg "Proposed model")  

## CIFAR10
Comparison between generated images by vanilla GAN generator and 1500 steps of MCMC  applied to generator output with step size 2.

For vanilla GAN model we dealed with zero discriminant loss problem -- for every iteration we see this noisy image.

![GAN](https://github.com/v-vskv-v/GAN_EBM/blob/master/cifar10/GAN/step21000.jpg "Vanilla GAN")

For proposed generative model we see movements in learned modes with different patterns in generated images.

![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/cifar10/GAN_EBM/step29000.jpg "Proposed model") ![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/cifar10/GAN_EBM/step12000.jpg "Proposed model") ![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/cifar10/GAN_EBM/step20000.jpg "Proposed model") ![GAN_EBM](https://github.com/v-vskv-v/GAN_EBM/blob/master/cifar10/GAN_EBM/step30000.jpg "Proposed model") 

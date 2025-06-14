AutoEncoder(AE) is a generative ai architecture that learns the representation of input data and projects it into a latent space and reconstructs the original input from the latent representation. It is a type of neural network that is trained to minimize the reconstruction error between the input and the output.

the architecutre is as follows: 

![image](img/autoencoder-architecture.png)

it uses MSE loss which is given as:
$$L(x,y) = \frac{1}{n}\sum_{i=1}^{n}(x_i - {y}_i)^2$$

for intuition we can see the latent space as 2D space and lets say we are training on the MNIST dataset, so everytime we encounter a "1" it should cluster at the same place in the latent space, the model will try to cluster the information by every epoch, it will learn some new representations 


note : **reconstruction quality = latent space quality** 

as we will increase the latent space size the reconstruction quality will increase but there should be a good threshold where it stops

visual demonstration from [deepia](https://www.youtube.com/@Deepia-ls2fo) youtube channel:

![alt text](image.png)
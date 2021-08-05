![van-gogh-header](https://user-images.githubusercontent.com/7725659/128417172-6da5c14c-0aa4-4996-ac8e-5ebb1c04a029.jpg)

# Portrait-Genre-GANs
Using Generative Adversarial Networks to transform portraits from one artistic genre to another. 

https://www.noahrush.com/public/pdfs/ML2020.pdf

## About
A project for Cornell Tech's fall Applied Machine Learning class in which we merge the ideas of creating Monet's using a cycleGAN (https://www.kaggle.com/c/gan-getting-started) with recent research into the StarGAN architecture (https://arxiv.org/abs/1711.09020). In our systems we start with portraits across a variety of artistic genres (Pointillism, Expressionism, etc..) and photographs of peoples faces, and try and learn transformations between them to generate new art or fake photographs. 

![pointil](https://user-images.githubusercontent.com/7725659/128417231-c09d0a22-561f-463a-85dc-402cb3f2b6fc.png)
(A pointillism painting generated from a real photograph)

The repo has two main files, cycleGAN and portrait Stargan, which do the two main parts of the project. The cycleGAN notebook allows the user to pick an artistic genre, and convert back and forth between a photo and that genre. StarGAN allows a lot of learning all at once, as it randomly selects genres to convert each training art to, and thus learns a bunch of transformations between many genres at once. 

## Data

The paintings come from the Painter by numbers competition on kaggle (https://www.kaggle.com/c/painter-by-numbers). We take only the artworks tagged as portraits. We also used images of groups, from http://chenlab.ece.cornell.edu/people/Andy/ImagesOfGroups.html. Before we enter the pictures into our models, we use a simple face recognition algorith to crop the images around the faces.

## Some Results
![27-images](https://user-images.githubusercontent.com/7725659/128418645-de711195-7c65-479a-82b3-2e78c47e566a.jpg)
![16-images](https://user-images.githubusercontent.com/7725659/128418649-81004048-d830-4d07-af9d-050b527eb0ae.jpg)



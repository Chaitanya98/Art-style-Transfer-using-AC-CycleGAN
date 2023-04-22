# Art Style Transfer using AC CycleGAN

![last commit](https://img.shields.io/github/last-commit/Chaitanya98/Art-Style-Transfer-using-AC-CycleGAN)
![repo size](https://img.shields.io/github/repo-size/Chaitanya98/Art-Style-Transfer-using-AC-CycleGAN)

The main objective of this project is to transform ordinary photos into beautiful works of art.

#

The aim of this project is to:

1. Acquire the ordinary images and images of each art style using the tensorflow datasets package.
2. Perform an exploratory data analysis to visualize a random sample of images from each art style. This analysis helps us to identify the differences and similarities between the images. Additionally, calculate statistics such as mean, standard deviation, histograms to understand the pixel distribution and color compositions of each art style.
3. Preprocess the images and prepare them for training.
4. Implement an Auxiliary Classifier CycleGAN using the CycleGAN network architecture described in the [paper](https://www.cs.cmu.edu/~junyanz/projects/CycleGAN/CycleGAN.pdf) to enable the model to learn the mapping between photographs and paintings along with the auxiliary information, which would be the desired art-style. This auxiliary information (i.e., the class labels) is incorporated into the CycleGAN network as an additional input. Finally, perform image-to-image translation using preprocessed image sets as inputs to the model and fine-tune it accordingly. Build the model such that we can mix the art-styles by using a continuous valued label.
5. Evaluate the model by visual inspection and FID scores and plot the progression of the images from one art-style to another.

#

Results:

![alt-text](https://github.com/Chaitanya98/Art-style-Transfer-using-AC-CycleGAN/blob/main/Images/Results-Sample.png?raw=True)

![alt-text](https://github.com/Chaitanya98/Art-style-Transfer-using-AC-CycleGAN/blob/main/Images/Art-style%20Progression.png?raw=True)





#

This repository contains,

- A `Data` folder that comprises ordinary images and Monet and Ukiyo-e artworks downloaded via the Tensorflow Datasets package. These images are used for training our AC-CycleGAN model. Additionally, there is a sub-folder named `ModelWeights_and_Losses` that stores the model weights and a pickle file of our losses dictionary.
- `Image to Image Translation using AC-CycleGAN` jupyter notebook.
- An `Images` folder which contains images of our results.
- `Poster` and `Presentation` we have made for our project.

#

References:
1. [Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks (Jun-Yan Zhu et al.)](https://arxiv.org/abs/1703.10593)
2. [Image-to-Image Translation with Conditional Adversarial Networks (Phillip Isola et al.)](https://arxiv.org/abs/1611.07004v3)
3. [Perceptual Losses for Real-Time Style Transfer and Super-Resolution (Justin Johnson et al.)](https://arxiv.org/abs/1603.08155)

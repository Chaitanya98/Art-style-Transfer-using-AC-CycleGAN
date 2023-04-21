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


# Face Generation
Face generation using Generative Adversarial Networks (GAN).  This project is part of the Udacity Deep Learning Nanodegree.

# Introduction

In this project, we'll define and train a DCGAN on a dataset of celebrity faces. Our goal is to get a generator network to generate new images of faces that look as realistic as possible!

The project will be broken down into a series of tasks from loading in data to defining and training adversarial networks. At the end of the notebook, we'll be able to visualize the results of your trained Generator to see how it performs; generated samples should look like fairly realistic faces with small amounts of noise.

We'll be using the [CelebFaces Attributes Dataset (CelebA)](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) to train the Generative Adversarial Network (GAN).

# Instructions

1. Set up the Jupyter ipython notebook environment
2. Load and visualize the images
3. Preprocess the images using dataloaders in pytorch
4. Define the GAN model architecture (Generator and Discriminator)
5. Build the complete GAN model using pytorch
6. Train the GAN model
7. Generate faces using the trained GAN model

## 1. Set up the Jupyter ipython notebook environment
## 1.1 Installation

* Download [Anaconda](https://www.anaconda.com/distribution/#download-section)

* Install [Anaconda](https://docs.anaconda.com/anaconda/install/) 

## 1.2 Create and Activate the Environment

Please go though this [doc](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) before you creating an environment.
After that create a environment using following command:

```
conda create --name deep-learning
```

Then activate the environment using following command:

```
activate deep-learning
```

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```

**Now, you can create a local version of the project**

1. Clone the repository, and navigate to the downloaded folder. 
```
git clone https://github.com/sureshsubr/generate-faces.git
cd generate-faces
```

2. Install PyTorch and torchvision; this should install the latest version of PyTorch.
	
	- __Linux__ or __Mac__: 
	```
	conda install pytorch torchvision -c pytorch 
	```
	- __Windows__: 
	```
	conda install pytorch -c pytorch
	pip install torchvision
	```

3. Install a few required pip packages, which are specified in the requirements text file.
```
pip install -r requirements.txt
```
Or
```
conda install --yes --file requirements.txt
```

4. That's it! Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.
```
jupyter notebook
```

Once jupyter notebook instance is open follow the remaining instructions steps #2 - #7 in the ipython notebook called `dlnd_face_generation.ipynb`.

To exit the environment when you have completed your work session, simply close the terminal window.

__NOTE:__ In the notebook, you will need to train the GAN in PyTorch.  If your GAN is taking too long to train, feel free to pursue the options under the section __Accelerating the Training Process__ below.



#### (Optionally) Accelerating the Training Process 

If your code is taking too long to run, you will need to either reduce the complexity of your chosen GAN architecture or switch to running your code on a GPU.  If you'd like to use a GPU, you can spin up an instance of your own, for example, you can use Amazon Web Services to launch an EC2 GPU instance but note that this costs money!!


# Image-Classification-TF

Image classification using a Inception v3 or Mobilenet model trained on ImageNet images,
and train a new top layer that can recognize other classes of images.

The top layer receives as input a 2048-dimensional vector (1001-dimensional for Mobilenet) for each image. We train a
softmax layer on top of this representation. Assuming the softmax layer contains N labels, this corresponds to
learning N + 2048*N (or 1001*N)  model parameters corresponding to the learned biases and weights.


### Create the virtual environment:

conda env create -f cvenv_macos.yml

### Activate the virtual environment:

conda activate cvenv

### Put labeled data in 'training_images'

Create a directory “(repository_location)\training_images”, then create a directory for each classification

Notes: 
1. at least 105 images of each type.
2. The images can be different sizes, but should be roughly square, and not especially large or small (i.e. substantially bigger than 50 x 50 and substantially smaller than 4000 x 4000).

### test_images:

Create a directory “(repository_location)\test_images”

### Run retrain.py

Note: that there are more than 20 parameters that can be specified, which allows for a great variety of customization options, however the defaults that I’ve chosen should be good to start with.

### Run test.py


# Image-Classification-TF


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


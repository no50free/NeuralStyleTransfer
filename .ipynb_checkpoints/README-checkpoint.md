# NeuralStyleTransfer
Some files and a Jupyter notebook allowing one to create new images in the style of famous artwork.

This repository and Jupyter notebook entitled "Neural Style Transfer". The other repository files are:
- A folder entitled 'images'. This is where you can add your own images to run the model on.
- A folder entiteld 'output'. This is where the saved images will appear, as well as the final generated image. 
- A script entitled 'nst_utils1.py' that contains some useful functions used in the notebook.
- A licencing agreement entiltled 'Pretrained_Model_LICENSE.txt' outlining the usage agreement for the pre-trained model.

In order to run the notebook on a local machine, it is necessary to download a large file. This file is available at 

https://www.kaggle.com/teksab/imagenetvggverydeep19mat

## Some parameters to play with
The purpose of this notebook is for a user to be able to generate her/his own fun images, without needing knowledge or background of Convolutional Neural Networks. The notebook and code were adapted and modified from an assignment in the Convolutional Neural Networks online course offered by DeepLearning.AI through Coursera.

There are several parameters that a user can toy with that may change the output.
### Within the Jupyter notebook
- alpha and beta. These are parameters that weight the relative contributions to the overall cost function of the content cost and stylized cost, respectively.
- num_iterations. This is set at 200 by default. 200 iterations should give the user a good sense of the stylized image. However, higher iterations such as 1200-1500 will produce a more detailed and subjectively pleasing picture.
- STYLE_LAYERS. These are each set to 0.2. They should sum to 1. Increasing the lower style layers inserts low level features, such as shapes and lines into the content picture. Increasing the higher style layers inserts finer, more textured patterns into the content picture.

### Within the nst.utils1.py file.
- IMAGE.WIDTH and IMAGE.HEIGHT. These are set to 400 and 300, respectively. The user's input images need these pixel dimensions for the code to run. These numbers can be changed if the user desires, however in my experience, increases these numbers dramatically increases the computational time.
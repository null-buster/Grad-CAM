# Grad-CAM heatmap visualization tool
An application to predict and map attention heatpoints using pretrained VGG16 model for UI/UX development and A/B testing.

#Installing the required modules for running the project
To install the requirements from requirements.txt please run:

`pip install -r requirements.txt`

Alternatively the requirements could also be installed by running seperate pip commands for each entry in the requirements.txt file. This can be done as shown below.

`pip install numpy`

`pip install opencv-python`

`pip install imutils`

`pip install tensorflow`

## Instructions for running the scripts

The project primarily contains a custom module named `gradcammodule` and a script named `apply_gradcam.py` which is the primary script where the program execution starts. The output heatmap generated are stored in the root folder `GRAD-CAM` having filenames in the format `Result_NameofFile.jpg`.The directory `images` contains the testing images I used to generate the output heatmaps.

## To run image gaze tracking script

To get the vision output heatmap for a particular image fire up a terminal and run the following command.

`python apply_gradcam.py -i images/amazon.jpg`

Here the command line argument `i` or `--image` specifies the path to the input image.
After the script fires up, it open's up the `open-cv` window where the generated heatmap is vertically stacked along with the original image and the output heatmap.

A demo of the output produced is shown below.
![Result_amazon.jpg](https://github.com/null-buster/Grad-CAM/blob/master/Result_amazon.jpg)


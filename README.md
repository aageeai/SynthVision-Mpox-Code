
# MPOX Detection Model

This repository contains a deep learning model for detecting Monkeypox (MPOX) from images using a Vision Transformer (ViT) as the backbone. The model can classify images into three categories: 'MPOX', 'Normal', and 'Other'.

## Prerequisites

Before you run the model, ensure you have the following installed:
- Python 3.7 or later
- TensorFlow 2.x
- TensorFlow Addons
- vit_keras

You can install the necessary libraries using:

```bash
!pip -q install vit_keras
!pip -q  install tensorflow-addons
```

## Model Weights

Download the model weights from the provided link and save them in your directory. Update the `mpox_model_WEIGHTS_PATH` in the script with the path to the downloaded weights.

## Usage

To use the model to predict on new images, follow these steps:

1. Update the `image_path` variable in the script to the path of the image you want to test.
2. Run notebook. The output will display the image along with its predicted class and the confidence score of the prediction.


## Script Overview

The script `mpox_model_predict.py` includes the following functionalities:
- Loading the ViT model pre-trained on ImageNet with the top layer customized for our three classes.
- A function `mpox_predict` that handles image preprocessing, model prediction, and visualization of results.


## License

Specify the license under which your project is released. This informs users how they can legally use the project's code.


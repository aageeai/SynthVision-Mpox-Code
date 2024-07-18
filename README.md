
# MPOX Detection Model

This repository contains a deep learning model for detecting Monkeypox (MPOX) from images using a Vision Transformer (ViT) as the backbone. The model can classify images into three categories: 'MPOX', 'Normal', and 'Other'. The 'MPOX' class used in this model is based entirely on 100% synthetic data.

## Model Training Dataset

The model was trained using the Mpox dataset, which consists of 1,000 synthetic clinical images generated with our proprietary SynthVision data generation pipeline. The dataset is specifically designed for Mpox digital detection research. It includes comprehensive coverage of lesions in various stages of the disease on different body parts, ensuring a diverse and comprehensive set of images. The dataset features representations of three different skin types, classified according to the Fitzpatrick scale. All images in the dataset are 100% synthetic. For more information, visit the dataset repository: [SynthVision-Mpox](https://github.com/aageeai/SynthVision-Mpox).

## Prerequisites

Before you run the model, ensure you have the following installed:
- Python 3.8 - 3.10 
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



## License

Specify the license under which your project is released. This informs users how they can legally use the project's code.


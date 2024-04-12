# Image Captioning Model

This project implements an image captioning model using deep learning techniques. The model is trained on the Flickr8k dataset and uses a pre-trained InceptionV3 model for image feature extraction and a stacked bi-directional GRU layer for caption generation.

## Data
The dataset used for this project is the Flickr8k dataset, which contains 8092 images in jpeg format. Each image is accompanied by 5 descriptions.

- [Flickr8k Dataset]()
- [Flickr8k Text]()

## Model
The model is built and trained using Keras. It consists of two main components:

1. **Image Feature Extraction:** A pre-trained InceptionV3 model is used to extract features from the images. The last layer of the model is removed and the output of the second last layer is used as the image features.

2. **Caption Generation:** A stacked bi-directional GRU layer is used to generate captions. The input to this layer is the image features and the pre-trained fasttext embeddings of the captions. The model predicts the next word till the end of the caption using greedy search during testing.

## Results
The trained model is able to generate captions for real-world images. The captions are not perfect but they are able to capture the main objects and actions in the image.

## To Do
- Add attention to the model to improve the quality of the captions.
- Use beam search instead of greedy search during testing.

## Usage
To use the model, first download the dataset and the trained weights. Then, run the **'image_captioning_model.ipynb'** notebook. The notebook contains code to load the dataset, preprocessing the images and captions, loading the trained weights, and generating captions for user given images.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Acknowledgments
- Flickr8k Dataset
- Flickr8k_text
- InceptionV3
- Python
- Jupyter Notebook- Numpy
- Pandas
- Matplotlib
- Tensorflow



# Automatic Image Captioning with Transformers and BLIP

# Overview

This repository contains an implementation of an automatic image captioning system leveraging the BLIP (Bootstrapped Language Image Pretraining) model, which integrates vision and language for effective image understanding. The project demonstrates end-to-end processing from dataset loading to model training and caption generation.

# Technical Requirements

* Transformers & Datasets: Utilized for handling pre-trained models and managing datasets.
* PyTorch: The primary deep learning library used for model creation and training.
* Hugging Face's Datasets: For streamlined data loading and preprocessing.
  
# Setup Instructions
To set up the environment, ensure that the transformers, datasets, and pytorch libraries are installed:

### pip install transformers datasets torch

# Dataset and Preprocessing
We use a football-themed dataset from Hugging Face's datasets library. The dataset is preprocessed and split into training sets to feed into the model for training:

* Load Dataset: Automatically downloads and splits the football dataset for training purposes.
* Image Captioning Dataset Class: Custom PyTorch Dataset class to encode and prepare images and captions for the model.
  
# Model Training and Evaluation
The project uses the BLIP model for image captioning, showcasing how to:

* Load the Pre-trained Model: Using BLIP from Salesforce's repository.
* Encode and Train: Custom function to encode images and captions, updating model parameters through training iterations.
* Generate Captions: Model evaluation by generating captions for new images.

# Usage
The notebooks guide users through each step of the project, from setting up the environment, loading and preprocessing the dataset, to training the model and generating captions for new images.

# Example Output
An example output of the project shows the model's capability to generate contextually relevant captions for football images, such as "Benzema after Real Madrid's win against PSG" and "Zidane with France in 2006 World Cup".

# Acknowledgments
Special thanks to Hugging Face for providing the datasets library and Salesforce for publishing the BLIP model.

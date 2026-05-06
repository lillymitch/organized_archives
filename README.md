# Project Proposal

## Group Members
Lilly Mitchell  
Zach Okayli-Masaryk  

## Abstract
This project addresses the problem of classifying artistic styles using image data. We will use artwork images from the WikiArt dataset and apply machine learning techniques, specifically image classification using convolutional neural networks, to classify each artwork into a simplified set of artistic style categories (e.g., Impressionism, Cubism, Baroque, Realism, Expressionism). Image features will be extracted using convolutional neural networks, and classifiers will be trained on these features. Success will be evaluated based on classification accuracy and analysis of model performance across artistic style categories.

## Motivation and Question
We have access to a large dataset of artwork images from the WikiArt dataset, including labeled artistic styles. Our motivation is to see whether visual features of an artwork can actually predict its artistic style.

This project explores whether machine learning can learn artistic and stylistic differences directly from images. A model like this could help museums, archives, or educational tools automatically categorize artworks by style.

## Planned Deliverables

### Full Success

We will create a Python codebase that includes:

* image loading and preprocessing  
* image augmentation and feature extraction  
* classification models that predict artistic style  

We will also create a Colab notebook that includes:

* dataset creation and cleaning  
* model training and evaluation  

Evaluation outputs will include:

* accuracy scores  
* a confusion matrix  
* basic error analysis  

The final system will take an image of an artwork as input and output a predicted artistic style category.

### Partial Success (Contingency Plan)

If the model does not perform well, we will still build a pipeline that includes:

* loading and preprocessing images  
* extracting features using convolutional neural networks  
* training classification models  

We will also:

* analyze limitations such as dataset size, class imbalance, or visually similar styles  

## Resources Required

### Data

* WikiArt dataset from Hugging Face  
  https://huggingface.co/datasets/huggan/wikiart  

The dataset includes images of artworks as features and artistic style labels as targets.

### Tools

* Python  
* pandas, numpy  
* pytorch  
* Google Colab  

## What You Will Learn

Through this project, we aim to learn:

* how to preprocess image data for deep learning  
* how convolutional neural networks learn visual features  
* how to apply classification models to image data  
* how dataset quality affects performance  
* how to build a full machine learning pipeline  

## Risk Statement

Limited or inconsistent image data  
Some artwork images may be low quality or difficult to classify visually  

Noisy or ambiguous style labels  
Some artistic styles overlap visually and may be difficult to separate  

To address this, we will:

* simplify artistic style labels  
* use image preprocessing and augmentation  
* start with a smaller, cleaner subset  

## Ethics Statement

If successful, this project could help improve how digital artwork collections are organized and accessed.

### Who benefits

* museums organizing digital archives  
* researchers and students  

### Who might be affected

* underrepresented artistic traditions if the dataset is biased  
* artworks that get misclassified  

We assume that visual features relate to artistic style and that automation improves access to knowledge.

Bias considerations include:

* overrepresentation of Western art  
* imbalance across artistic style categories  
* weaker performance on less common classes  

We will treat predictions as assistive, not definitive.

## Tentative Timeline

### Weeks 1-2 (now to April 26)

* load and explore dataset  
* preprocess images  
* clean and simplify labels  
* implement baseline models  
* train a convolutional neural network  

Goal: get a working baseline model

### Weeks 3-4 (April 27 to May 15)

* improve model  
* evaluate performance  
* perform error analysis

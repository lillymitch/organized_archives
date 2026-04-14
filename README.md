# Project Proposal

## Group Members
Lilly Mitchell  
Zach Okayli-Masaryk  

## Abstract
This project addresses the problem of organizing museum collections by predicting the medium of artworks using image data. We will use images associated with artworks from the Metropolitan Museum of Art dataset and apply machine learning techniques, specifically image classification using transfer learning, to classify each artwork into a simplified set of medium categories (e.g., oil painting, watercolor, ceramic). Image features will be extracted using a convolutional neural network, and a classifier will be trained on these features. Success will be evaluated based on classification accuracy and analysis of model performance across medium categories.

## Motivation and Question
We have access to a large dataset of museum artifacts from the Metropolitan Museum of Art, including images that can be retrieved via object IDs through the museum’s public API. Our motivation is to see whether visual features of an artwork can actually predict its medium.

This project explores whether machine learning can learn artistic and material differences directly from images. A model like this could help museums automatically categorize new or uncataloged works.

## Planned Deliverables

Full Success

We will create a Python codebase that includes a data acquisition pipeline (retrieving image URLs via the Met API), image preprocessing and feature extraction, and a classification model that predicts artwork medium.

We will also create a Colab notebook that shows how the dataset is created and cleaned, along with model training and evaluation.

Evaluation outputs will include accuracy scores, a confusion matrix, and basic error analysis (e.g., MSE).

The final system will take an image of an artwork as input and output a predicted medium category.

Partial Success (Contingency Plan)

If the model does not perform well, we will still build a working pipeline for retrieving and preprocessing images, extracting features using a pretrained model, and training a classifier.

We will analyze limitations such as dataset size, class imbalance, or unclear labels, and the final result will demonstrate a complete ML workflow and areas for improvement.

## Resources Required

Data

Metropolitan Museum of Art Open Access dataset  
https://github.com/metmuseum/openaccess  

Images retrieved via the Met Collection API using object IDs  

The dataset includes images of artworks as features and medium labels (simplified into categories) as targets.

Tools

Python  
pandas, numpy  
pytorch or tensorflow  
Google Colab  

## What You Will Learn

Through this project, we aim to learn how to collect and preprocess image data from an API, how to use pretrained convolutional neural networks, how to apply classification models to image data, how dataset quality affects performance, and how to build a full machine learning pipeline.

## Risk Statement

Limited or inconsistent image data: not all objects have images, and some may be low quality.

Noisy or ambiguous medium labels: the “Medium” field varies a lot and needs simplification.

To address this, we will filter for objects with valid images, simplify medium labels, and start with a smaller, cleaner subset of the data.

## Ethics Statement

If successful, this project could help improve how museum collections are organized and accessed.

Who benefits

Museums organizing digital archives  
Researchers and students  

Who might be affected

Underrepresented cultures if the dataset is biased  
Artifacts that get misclassified  

We assume that visual features relate to medium and that automation improves access to knowledge.

Bias considerations include overrepresentation of Western art, imbalance across medium categories, and weaker performance on less common classes. We will treat predictions as assistive, not definitive.

## Tentative Timeline

Weeks 1-2 (now to April 26)

Load and explore dataset  
Retrieve images  
Clean and simplify labels  
Extract features  
Train a basic model  

Goal: get a working baseline model

Weeks 3-4 (April 27 to May 15)

Improve model  
Evaluate performance  
Perform error analysis


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

We will create

* A Python codebase implementing
  * a data acquisition pipeline (retrieving image URLs via the Met API)
  * image preprocessing and feature extraction
  * a classification model that predicts artwork medium

* A Colab notebook demonstrating
  * dataset creation and cleaning
  * model training and evaluation

* Evaluation outputs including
  * accuracy scores
  * a confusion matrix
  * basic error analysis (e.g., MSE)

The final system will take an image of an artwork as input and output a predicted medium category.

Partial Success (Contingency Plan)

If the model does not perform well

* we will still build a working pipeline for
  * retrieving and preprocessing images
  * extracting features using a pretrained model
  * training a classifier

* we will look at limitations like dataset size, class imbalance, or unclear labels

* the final result will show a full ML workflow and where things could be improved

## Resources Required

Data

* Metropolitan Museum of Art Open Access dataset  
https://github.com/metmuseum/openaccess  

* images retrieved via the Met Collection API using object IDs  

features — images of artworks  
targets — medium (simplified into categories)  

Tools

* Python  
* pandas, numpy  
* pytorch or tensorflow  
* Google Colab  

## What You Will Learn

Through this project, we aim to learn

* how to collect and preprocess image data from an API  
* how to use pretrained convolutional neural networks  
* how to apply classification models to image data  
* how dataset quality affects performance  
* how to build a full ML pipeline  

## Risk Statement

Limited or inconsistent image data  
not all objects have images, and some may be low quality  

Noisy or ambiguous medium labels  
the “Medium” field varies a lot and needs simplification  

To deal with this

* filter for objects with valid images  
* simplify medium labels  
* start with a smaller, cleaner subset  

## Ethics Statement

If successful, this project could help improve how museum collections are organized and accessed.

Who benefits

* museums organizing digital archives  
* researchers and students  

Who might be affected

* underrepresented cultures if the dataset is biased  
* artifacts that get misclassified  

We assume that visual features relate to medium and that automation helps access.

Bias considerations

* dataset may overrepresent Western art  
* some mediums may dominate  
* performance may be worse on less common categories  

We will treat predictions as assistive, not definitive.

## Tentative Timeline

Weeks 1–2 (now → April 26)

* load and explore dataset  
* retrieve images  
* clean labels  
* extract features  
* train a basic model  

goal: get something working  

Weeks 3–4 (April 27 → May 15)

* improve model  
* evaluate performance  
* do error analysis  
* Evaluate performance (accuracy, confusion matrix)
* Perform error analysis
* Create visualizations
* Write final report and prepare notebook


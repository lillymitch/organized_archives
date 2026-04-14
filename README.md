Group Members: Lilly Mitchell and Zach Okayli-Masaryk
## Abstract
This project addresses the problem of organizing museum collections by predicting the medium of artworks using image data. We will use images associated with artworks from the Metropolitan Museum of Art dataset and apply machine learning techniques, specifically image classification using transfer learning, to classify each artwork into a simplified set of medium categories (e.g., oil painting, watercolor, ceramic). Image features will be extracted using a pretrained convolutional neural network, and a classifier will be trained on these features. Success will be evaluated based on classification accuracy and analysis of model performance across medium categories.
## Motivation and Question
We have access to a large dataset of museum artifacts from the Metropolitan Museum of Art, which includes metadata and object IDs that can be used to retrieve associated images through the museum’s public API. While metadata provides useful information, visual characteristics are often more directly tied to an artwork’s medium. This motivates the question: To what extent can visual features of an artwork be used to accurately predict its medium? This project is interesting because it explores whether machine learning can learn meaningful artistic and material distinctions (e.g., paint vs. sculpture) directly from images. Such a model could help museums automatically categorize new or uncataloged works and improve digital organization systems.
## Planned Deliverables
Full Success
We will create:
* A Python codebase implementing:
 *     Data acquisition pipeline (retrieving image URLs via the Met API)
 *     Image preprocessing and feature extraction
 *     A classification model to predict artwork medium
* A Colab notebook demonstrating:
 *     Dataset creation and cleaning
 *     Model training and evaluation
* Evaluation outputs including:
 *     Accuracy scores
 *     Confusion matrix
 *     Basic error analysis
The final system will take an image of an artwork as input and output a predicted medium category.
Partial Success (Contingency Plan)
If the model does not perform well:
* We will still produce a working pipeline for:
 *     retrieving and preprocessing images
 *     extracting features using a pretrained model
 *     training a classifier
* We will analyze limitations such as dataset size, class imbalance, or ambiguous labels
* The final deliverable will demonstrate a complete ML workflow and identify areas for improvement
## Resources Required
Data:
* Metropolitan Museum of Art Open Access dataset:
https://github.com/metmuseum/openaccess
* Images retrieved via the Met Collection API using object IDs
The dataset includes:
* features: images of artworks
* targets: medium (which we will simplify into categories)
Tools:
* Python
* pandas, numpy
* scikit-learn
* (optional) PyTorch or TensorFlow for image feature extraction
* Google Colab
## What You Will Learn
Through this project, we aim to learn:
* How to collect and preprocess image data from an external API
* How to use pretrained convolutional neural networks for feature extraction
* How to apply classification models to image-based data
* How dataset quality and labeling affect model performance
* How to build a complete machine learning pipeline involving real-world data
## Risk Statement
Limited or inconsistent image data
 Not all objects have images, and some image URLs may fail or be low quality.
Noisy or ambiguous medium labels
 The “Medium” field is highly variable (e.g., “oil on canvas,” “oil on wood”), requiring simplification that may introduce errors.
To mitigate these risks:
* We will filter for objects with valid images
* Simplify medium labels into a small number of categories
* Work with a manageable subset of the dataset
## Ethics Statement
If successful, this project could improve the organization and accessibility of museum collections by automating aspects of artifact classification.
Who benefits:
* Museums organizing digital archives
* Researchers and students studying art and cultural artifacts
Who might be excluded or harmed:
* Underrepresented cultures if the dataset is biased toward certain regions or traditions
* Communities whose artifacts are misclassified due to model limitations
Assumptions:
Visual features of artworks correlate meaningfully with their medium
Automating classification improves access to cultural knowledge
Bias considerations:
* The dataset may overrepresent Western art traditions
* Some media types may dominate the dataset, leading to class imbalance
* The model may perform poorly on less-represented categories
We will acknowledge these limitations and treat predictions as assistive rather than authoritative.
## Tentative Timeline
Weeks 1-2 (now → April 26):
* Load and explore dataset
* Retrieve images using the API for a subset of objects
* Clean and simplify medium labels
* Extract image features using a pretrained model
* Train a basic classifier
Goal: produce a working baseline model with initial results
Weeks 3-4 (April 27-May 15)
* Improve model (tuning, better feature selection)
* Evaluate performance (accuracy, confusion matrix)
* Perform error analysis
* Create visualizations
* Write final report and prepare notebook


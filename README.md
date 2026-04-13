# organized_archives
Organizing artifact archives by certain classifiers
## Group Members

Lilly Mitchell and Zach Okayli-Masaryk
## Abstract
This project addresses the problem of organizing museum collections by predicting the time period of artworks using metadata. We will use text-based features such as descriptions, materials, and object types from open-access museum datasets and apply machine learning models like logistic regression or Naive Bayes to classify each artwork into a predefined historical period. Text data will be converted into numerical features using TF-IDF vectorization. Success will be evaluated based on classification accuracy and analysis of model performance across different time periods.
## Motivation and Question
We have data from art museums that can be used to predict artwork classifications with our models. The artwork in the dataset already has classifiers, so we can drop those columns, predict the classification, and compare it to our y_test (the dropped columns). This is motivating because we have access to an abundance of information, giving us more flexibility to be creative and have fun. Our scientific question is, “To what extent can metadata (such as descriptions, materials, and type) be used to accurately predict the time period of artworks and artifacts?
## Planned Deliverables
We will create a Python package that pipelines a machine learning algorithm and model to predict the classification of artwork based on metadata from the Metropolitan Museum of Art. We will include a data processing function, use feature extraction techniques, and implement model training and loss evaluation.
We will use a Google Colab notebook to demonstrate how to use our pipeline, with text written above the code that explains what each section does. The pipeline will include visualizations, such as a confusion matrix, to make our model's success more visible and comprehensible. 
Our model’s performance will be evaluated using a loss function, such as mean squared error, and its success will be measured by accuracy.
If we achieve complete success, we would, in theory, have a model with a low mean-squared error on the test data, as well as a well-commented notebook that shows how to use the pipeline and describes what each section aims to achieve. 
If the model does not work as planned, our deliverable will be a pipeline displaying our learning throughout the process. We will document our work in Google Colab, making it easy to return to in the future. We will have a foundation to build a better model on and know which techniques to replace our old model with. We will also learn how a better dataset can lead to an improved deep learning model.
## Resources Required
Data: We plan to use the Metropolitan Museum of Art open-access dataset at https://github.com/metmuseum/openaccess/blob/master/MetObjects.csv. These datasets include both features (descriptions, materials, object types) and targets (dates or time periods, which we will group into categories).

Tools: Python, scikit-learn, pandas, numpy, and Google Colab

Computing: Personal laptop
## What You Will Learn
Through this project, we aim to learn how to preprocess and clean real-world textual data, how to apply Term Frequency-Inverse Document Frequency for feature extraction, how dataset quality impacts ML performance, and how to structure a complete ML pipeline from raw data to evaluation. 
## Risk Statement
It is possible that metadata alone does not strongly correlate with time period, leading to low model accuracy. Secondly, museum datasets may contain inconsistent, missing, or ambiguous date information, making it difficult to define clear target labels. To mitigate these risks, we will simplify the time-period categories, filter out incomplete records, and start with a small, clean subset of the data. 
## Ethics Statement
If successful, this project could help improve access to and organization of museum collections, benefiting researchers, students, and the general public.
Who benefits:
  Museums seeking to organize digital archives
  Researchers and students exploring cultural artifacts
Who might be excluded or harmed:
  Underrepresented cultures, if datasets are biased toward Western collections
  Communities whose artifacts are misclassified or misinterpreted
Assumptions:
  Metadata contains meaningful signals about historical context
  Improving the organization of museum data leads to broader access to knowledge
Bias considerations:
  Museum datasets may reflect historical and colonial biases
  Certain time periods or cultures may be overrepresented
  The model may perform better on well-represented groups
We will acknowledge these limitations and treat predictions as assistive, not authoritative.
## Tentative Timeline
Weeks 1-2 (now → April 26):
  Obtain and inspect dataset
  Clean and preprocess data
  Define time period categories
  Implement basic TF-IDF + simple model
  Goal: produce a working baseline model with initial results
Weeks 3-4 (April 27-May 15)
  Improve model (tuning, feature selection)
  Evaluate performance (accuracy, confusion matrix)
  Conduct error analysis
  Create visualizations
  Write the final report and prepare the notebook

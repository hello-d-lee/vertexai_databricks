# vertexai_databricks
options for training, testing, deploying models trained on either GCP products (AutoML, BQML, Vertex notebooks) or Databricks. end to end for online prediction example, same training dataset used.

# Overview
These notebooks will demonstrate the different ways to train a model in various services (AutoML, BQML, Databricks) and export that model to the model registry to deploy it on a Vertex AI endpoint for online prediction

* Setup notebook - required infrastructure and datasets that will be used in the subsequent notebooks
* AutoML notebook - train a Vertex AI AutoML model, and then get the parameters for that model from the logs after training
* BQML notebook - train model using BigQuery ML, check the artifacts and export to the Vertex AI model registry 
* Databricks notebook - train the model in a Databricks notebook, then use the webhook to export that model to Vertex AI model registry
* Vertex Workbench managed notebook - how to train the model using Vertex AI's managed notebooks
* Deployment & cleanup notebook - create an endpoint for each type of model, deploy each model to the endpoint, test the prediction service. Finally, delete running resources to avoid incurring extra costs.  

As a next step, show how to use Vertex AI pipelines for end to end MLOps orchestration 

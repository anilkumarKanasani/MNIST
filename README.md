---
page_type: sample
languages:
- python
products:
- azure
- azure-machine-learning-service
- azure-devops
description: "Code which demonstrates how to set up and operationalize an MLOps flow leveraging Azure Machine Learning and Azure DevOps."
---

# DeepLearning Models for (MNIST) Image Classification Problems

CI: [![Build Status](https://aidemos.visualstudio.com/MLOps/_apis/build/status/Model-Train-Register-CI?branchName=main)](https://aidemos.visualstudio.com/MLOps/_build/latest?definitionId=160&branchName=main)

CD: [![Build Status](https://aidemos.visualstudio.com/MLOps/_apis/build/status/microsoft.MLOpsPython-CD?branchName=main)](https://aidemos.visualstudio.com/MLOps/_build/latest?definitionId=161&branchName=main)

MLOps will help you to understand how to build a Continuous Integration and Continuous Delivery pipeline for an ML/AI project. We will be using the Azure DevOps Project for build and release/deployment pipelines along with Azure ML services for model retraining pipeline, model management and operationalization.

![ML lifecycle](/docs/images/ml-lifecycle.png)

This template contains code and pipeline definitions for a machine learning project that demonstrates how to automate an end to end ML/AI workflow.

## Architecture and Features

Architecture Reference: [Machine learning operationalization (MLOps) for Python models using Azure Machine Learning](https://docs.microsoft.com/en-us/azure/architecture/reference-architectures/ai/mlops-python)

This reference architecture shows how to implement continuous integration (CI), continuous delivery (CD), and retraining pipeline for an AI application using Azure DevOps and [Azure Machine Learning](/azure/machine-learning/service/overview-what-is-azure-ml). The solution is built on the scikit-learn diabetes dataset but can be easily adapted for any AI scenario and other popular build systems such as Jenkins and Travis.

The build pipelines include DevOps tasks for data sanity tests, unit tests, model training on different compute targets, model version management, model evaluation/model selection, model deployment as realtime web service, staged deployment to QA/prod and integration testing.

## Prerequisite

- Active Azure subscription
- At least contributor access to Azure subscription

## Getting Started

To deploy this solution in your subscription, follow the manual instructions in the [getting started](docs/getting_started.md) doc. Then optionally follow the guide for [integrating your own code](docs/custom_model.md) with this repository template.

### Repo Details

You can find the details of the code and scripts in the repository [here](/docs/code_description.md)

### References

- [Azure Machine Learning (Azure ML) Service Workspace](https://docs.microsoft.com/en-us/azure/machine-learning/service/overview-what-is-azure-ml)
- [Azure ML CLI](https://docs.microsoft.com/en-us/azure/machine-learning/service/reference-azure-machine-learning-cli)
- [Azure ML Samples](https://docs.microsoft.com/en-us/azure/machine-learning/service/samples-notebooks)
- [Azure ML Python SDK Quickstart](https://docs.microsoft.com/en-us/azure/machine-learning/service/quickstart-create-workspace-with-python)
- [Azure DevOps](https://docs.microsoft.com/en-us/azure/devops/?view=vsts)

## Source

This project is adopted from Microsoft official MLOps Template. Please visit the below website for more details about the source template
https://github.com/microsoft/MLOpsPython
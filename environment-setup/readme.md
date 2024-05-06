# SCENARIO 1 - Azure environment

## Option 1 - Use provided sandbox Azure environment

https://aka.ms/rai-hub/dashboard-workshop

## Option 2 - Bring your own environment

1) Create Azure Machien Learning Workspace
2) Create a Compute Instance (default settings)
3) Go to NOTEBOOKS
4) Open TERMINAL
5) Clonee the REPO 
- TIP: If you clone with "SPARSE CHECKOUT" it goes quicker
```python
# Clone the repository into a new directory
git clone --no-checkout --filter=blob:none --branch main https://github.com/Azure/azureml-examples.git
# Navigate into the new directory
cd azureml-examples

# Initialize sparse-checkout
git sparse-checkout init --cone

# Set the directories you want to check out
# Replace <dir> with the directory you want
git sparse-checkout set <dir>

# Pull the files
git pull origin main

```

6) Choose scenario - Recommended scenarios: 
    - TABULAR: 
        - "Housing": Classification
            - https://github.com/Azure/azureml-examples/blob/main/sdk/python/responsible-ai/tabular/responsibleaidashboard-housing-classification-model-debugging/responsibleaidashboard-housing-classification-model-debugging.ipynb
        - "Healthcare - Covid" : Classification
            - https://github.com/Azure/azureml-examples/blob/main/sdk/python/responsible-ai/tabular/responsibleaidashboard-healthcare-covid-classification/responsibleaidashboard-healthcare-covid-classification.ipynb
    - TEXT:"Financial news": Classification
        - https://github.com/Azure/azureml-examples/blob/main/sdk/python/responsible-ai/text/responsibleaidashboard-text-classification-financial-news/responsibleaidashboard-text-classification-financial-news.ipynb

    - IMAGE: "Fridge items": Classification, Object detection
        - https://github.com/Azure/azureml-examples/blob/main/sdk/python/responsible-ai/vision/responsibleaidashboard-image-classification-fridge.ipynb
        - https://github.com/Azure/azureml-examples/blob/main/sdk/python/responsible-ai/vision/responsibleaidashboard-object-detection-MSCOCO.ipynb

7) 
7) Configure a ntoebook with your Azure information
- Azure subscription ID
- Azure Machine Learning workspace ID
- Resource Group

```Python

subscription_id = "<SUBSCRIPTION_ID>"
resource_group = "<RESOURCE_GROUP>"
workspace = "<AML_WORKSPACE_NAME>"

```

8) Run the notebook.
If any errors or trouble - get in contact with the mentors.




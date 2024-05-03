
# SCENARIO 2: `Generative AI` evaluation in `AI studio` with RAG for: Chatbots, GenAI solutions

### DATA
- PRODUCT DATA for "on your data", e.g. RAG to create index on: [../../data/scenario-2-genai/3-product-info/ ](../../data/scenario-2-genai/3-product-info/)
- CUSTOMER DATA for "on your data", e.g. RAG to create index on: [../../data/scenario-2-genai/1-customer-info/](../../data/scenario-2-genai/1-customer-info/)
- EVALUATION DATA: [../../data/scenario-2-genai/6-evaluation-jsonl](../../data/scenario-2-genai/6-evaluation-jsonl/)


# About this lab
In this lab we will explore the generative AI evaluation dashboard in Azure AI Studio. You will first build a RAG application based on some sample data. It is basically a chatbot for **Contoso Outdoor shop** and you can ask questions regarding the product catalog as well as customer purchase histories.

# Task 1:Set up your project in Azure AI Studio
As prerequisite for this lab you need to set up a project in Azure AI Studio(https://ai.azure.com/) and provision the required resources.

Make sure you have created the following resources:
- An Azure OpenAI resource
- An AI search resource
  
You'll need to deploy a chat completions model (e.g. GPT-3.5-turbo 1106) and a text embedding model (e.g. text-embedding-ada-002). Do this in the "deployment" tab in your AI studio project.

# Task 2:Build the search indexes using the playground 
1. Go to **Tools-->Playground** in the sidebar. You will use the built-in "**Add your data**" functionality to add your data sources and build an index for it in Azure AI search.
2. Click on "'**+Add a new data source**" button, select "Upload files" where you choose all the documents in the PRODUCT DATA folder. Build an index called e.g. "product-index".
3. After the process finishes, you could test your chatbox in the playground by providing question such as "How much does TrailMaster cost?". The answer should provide a price with a reference to the data that you have grounded the application with in the previous step. You could take a look at some product documents and ask questions accordingly to test that your RAG application is working.
4. Repeat step 2-3 but this time build another index called e.g. "customer-index" using CUSTOMER DATA.

# Task 3:Test manual evaluation feature 

# Task 3:Create a prompt flow for product-index only

# Task 4:Run RAI evaluation for product-index only flow

# Task 5:Create a prompt flow for multi-indexes

# Task 6:Run RAI evaluation for multi-indexes flow

# Task 7:Compare the two evaluation results

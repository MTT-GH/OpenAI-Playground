# OpenAI-Playground

## Deploy the Azure resources
Depending on the demo used, you will need to deploy some of the following Azure Resources :
- Azure OpenAI service
- Azure Speech
- Azure Computer Vision
- Azure Search 
- Azure Document Intelligence (old Form Recognizer)

## Prepared to run in GitHub Codespace (also local devcontainer)

The repository has been prepared to execute as a devcontainer (using GitHub Codespaces). This container includes all the tools needed (mainly Python/Jupyter) and python libraries. You can check the deployed configuration in:
- [Devcontainer folder](.devcontainer/devcontainer.json)
- [Requirements file for Python libraries](requirements.txt)

### Add GitHub Codespace secrets

Add the following secrets related to the deployed Azure resources to the GitHub Repository (Codespaces), as they are going to be used in the Demos (**some demos may require more settings**). Go to **Settings>Secrets and Variables>Codespaces**: 


![Alt text](Settings.png)

For **Azure OpenAI**
- AZURE_OPENAI_API_KEY
- AZURE_OPENAI_ENDPOINT
- AZURE_OPENAI_MODEL_CHAT: In my case I used a deployment of "gpt-35-turbo"
- AZURE_OPENAI_MODEL_CHAT_VERSION : in my case I used "2023-03-15-preview"
- OPENAI_ADA_EMBEDDING_DEPLOYMENT_NAME Your "text-embedding-ada-002" model deployment name
- OPENAI_ADA_EMBEDDING_MODEL_NAME = text-embedding-ada-002

For **Azure Search**
- AZURE_SEARCH_ADMIN_KEY
- AZURE_SEARCH_SERVICE_ENDPOINT
- AZURE_COGNITIVE_SEARCH_SERVICE_NAME

For **Azure Computer Vision**
- AZURE_COMPUTER_VISION_ENDPOINT
- AZURE_COMPUTER_VISION_KEY

For **Azure Document Intelligence** (Form Recognizer)
- AZURE_DOC_ENDPOINT
- AZURE_DOC_KEY

For **Azure Speech**
- AZURE_SPEECH_KEY
- AZURE_SPEECH_REGION

## Demos 

- The GitHub codespace automatically installs all needed modules when launched, but you can also find them in the **requirements.txt** file.
    > WARNING: you can also execute "pip3 install --user -r requirements.txt" if the libraries are missing for some reason.
- For the jupiter Notebooks, open the file and **select kernel** before running (**python 3.11 is provided**). Configuration can be given in two ways:

    1. Using GitHub Codespace and secrets ( **PREFERRED**, as show above)
    2. Provide an ".env" file (commented in many files)

### Basics 

The following demos are provided under the [DeepLearningAI-Course](OpenAI/DeepLearningAI-Course) folder. Demos are taken from the course provided at https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/1/introduction . All Demos use **ChatCompletion** Endpoint. 

- [Getting Started](OpenAI/DeepLearningAI-Course/l2-guidelines.ipynb)
- [Iterative Prompts](OpenAI/DeepLearningAI-Course/l3-iterative-prompt-development.ipynb)
    - Create Description from Product Fact Sheet (limit words, focus on aspects, add dimension, render into an HTML page)
- [Summarizing](OpenAI/DeepLearningAI-Course/l4-summarizing.ipynb)
    - Summarize various product reviews in a single prompt
- [Inferring](OpenAI/DeepLearningAI-Course/l5-inferring.ipynb)
    - Analyze text sentiment, emotions, identify anger (product review), extract product information, ...
- [Transforming](OpenAI/DeepLearningAI-Course/l6-transforming.ipynb)
    - Translate single and multiple languages, using different tones
    - Format conversion (JSON to HTML)
    - Grammar checks
- [Expanding](OpenAI/DeepLearningAI-Course/l7-expanding.ipynb)
    - Automate email reply to customers reviews
- [ChatBot](OpenAI/DeepLearningAI-Course/l8-chatbot.ipynb)
    - Provide multiple messages (with roles), to the "ChatCompletion" call.
    - Pizza ordering Bot sample

### Intermediate

- [Speech Summarizing with OpenAI and Azure Speech AI](OpenAI/Speech-Summarize/Speech-summarizing.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
- [Open AI and Azure Document Intelligence (Form Recognizer)](OpenAI/Document-Intelligence/Document-Intelligence.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
    - Use Form Recognizer for Image to Text, and use "text-davinci" AOAI model to summarize.
- [Gradio webapp with Azure ChatGPT, your own chatGPT website](OpenAI/Gradio-ChatBot-WebApp/Gradio-WebApp-ChatGPT.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)

- [Use OpenAI with your own data](OpenAI/OpenAI-YourData/README.md)

- [Azure Computer Vision and Langchain](OpenAI/ComputerVision-Langchain/computer-vision-langchain.ipynb) taken and modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)


### Advanced
- [Functions calling with Azure Open AI and Azure Search ]() TODO taken & modified from [repo](https://github.com/Azure-Samples/openai/tree/main/Basic_Samples/Functions)
- [Movie recommender with Azure Open AI & Azure  Search]() taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
    - Part 1:  Embeddings generation with Azure Open AI and Azure Cognitive Search ingestion
    - Part 2: Search examples 
        - Section 3 search queries : vector, with filters, hybrid, semantic, ...
        - Section 6 Mixes OpenAI GPT with Azure Search
        - Section 7.2 **Runs a webapp with the solution!**
    - Part 3: Recommandations
    ![Movie Recommender](OpenAI/Movie-recommender/architecture.png)

- [Code Analysis with with Langchain + Azure OpenAI + Azure Cognitive Search (vector store)](OpenAI/CodeAnalysis-Langchain-AOAI-Search) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)

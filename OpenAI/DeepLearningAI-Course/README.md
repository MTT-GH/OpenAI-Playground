# ChatGPT Prompt Engineering for Developers - Azure OpenAI Services Edition

## Samples taken from course at https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/1/introduction 

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/shirkey/deeplearning-ai-chatgpt-prompt-eng-azure-openai)

This repository is based on the source code shared in the [DeepLearningAI](https://www.deeplearning.ai) fantastic and free short course of [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/).

Changes have been made to the original source code to accommodate the use of [Azure OpenAI (AOAI) Services](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/) Services as an alternative to OpenAI's own endpoints.

## Setup

- Sign-up for the [course](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
- Create your Azure OpenAI Services Resource and Model Deployment -- refer to docs [here](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/create-resource?pivots=web-portal)
    - Choose from `eastus`, `southcentralus` or `westeu` as the region where AOAI services are currently available (as of 29/04/2023)
    - Deploy the `gpt-35-turbo` model, naming it either `gpt-35-turbo` or another name (updating .env to reflect the same)
    
## Running the Code

### OPTION 1: Launch in Github Codespaces
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/shirkey/deeplearning-ai-chatgpt-prompt-eng-azure-openai)
- Run the notebooks:
    - `jupyter notebook` then select the specific tutorial notebook (eg l2 -> l8)
- Watch the course videos and follow along with each related notebook

### OPTION 2: 
- Clone this repository to a local machine
- Install the required Python modules:
    - `pip install -r requirements.txt`
- Run the notebooks:
    - `jupyter notebook` then select the specific tutorial notebook (eg l2 -> l8)
- Watch the course videos and follow along with each related notebook

# OpenAI-Playground

## Prepared to run in GitHub Codespace (also local devcontainer)

Add the following secrets to the GitHub Repository (Codespaces), as they are going to be used in the Demos (**some demos may require more settings**):

![Alt text](Settings.png)

- AZURE_OPENAI_API_KEY
- AZURE_OPENAI_ENDPOINT
- AZURE_OPENAI_MODEL_CHAT: In my case I used a deployment of "gpt-35-turbo"
- AZURE_OPENAI_MODEL_CHAT_VERSION : in my case I used "2023-03-15-preview"

## Demos 

- The GitHub codespace automatically installs all needed modules when launched, but you can also find them in the *requirements.txt* file.
    > WARNING: you can also execute "pip3 install --user -r requirements.txt" if the libraries are missing for some reason.
- For the jupiter Notebooks, open the file and **select kernel** before running. Configuration can be given in two ways:

    1. Using GitHub Codespace and secrets (as show above)
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

- [Speech Summarizing with OpenAI and Azure Speech AI](OpenAI/Speech-Summarize/Speech-summarizing.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/blob/main/Azure%20Open%20AI%20quick%20demos/Azure%20Open%20AI%20-%20Demo%204%20Speech%20summarizing.ipynb)
- [Open AI and Azure Document Intelligence]() taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/blob/main/Azure%20Open%20AI%20quick%20demos/Azure%20Open%20AI%20-%20Demo%204%20Speech%20summarizing.ipynb)
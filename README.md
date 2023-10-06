
# OpenAI-Playground

Please give a star to the repository to support the initiative :star:

## Prerequisites

Follow the instructions at [Getting Started](Getting_Started.md)

## Available Demos 

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

- [Azure Function calling with Azure Open AI - Simple](OpenAI/Function-Calling-Simple/working_with_functions.ipynb) taken & modified from [repo](https://github.com/Azure-Samples/openai/tree/main/Basic_Samples/Functions)


### Intermediate

- [Speech Summarizing with OpenAI and Azure Speech AI](OpenAI/Speech-Summarize/Speech-summarizing.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
- [Open AI and Azure Document Intelligence (Form Recognizer)](OpenAI/Document-Intelligence/Document-Intelligence.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
    - Use Form Recognizer for Image to Text, and use "text-davinci" AOAI model to summarize.
- [Gradio webapp with Azure ChatGPT, your own chatGPT website](OpenAI/Gradio-ChatBot-WebApp/Gradio-WebApp-ChatGPT.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)

- [Use OpenAI with your own data](OpenAI/OpenAI-YourData/README.md)

- [Azure Computer Vision and Langchain](OpenAI/ComputerVision-Langchain/computer-vision-langchain.ipynb) taken and modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)

- **TODO** [Functions calling with Azure Open AI and Azure Search ]()  taken & modified from [repo](https://github.com/Azure-Samples/openai/tree/main/Basic_Samples/Functions)


### Advanced

- [Movie recommender with Azure Open AI & Azure  Search](OpenAI/Movie-recommender/) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
    - Part 1:  Embeddings generation with Azure Open AI and Azure Cognitive Search ingestion
    - Part 2: Search examples 
        - Section 3 search queries : vector, with filters, hybrid, semantic, ...
        - Section 6 Mixes OpenAI GPT with Azure Search
        - Section 7.2 **Runs a webapp with the solution!**
    - Part 3: Recommandations
    ![Movie Recommender](OpenAI/Movie-recommender/architecture.png)

- [Code Analysis with with Langchain + Azure OpenAI + Azure Cognitive Search (vector store)](OpenAI/CodeAnalysis-Langchain-AOAI-Search) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)

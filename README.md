
# OpenAI-Playground

Please give a star to the repository to support the initiative :star:

## Prerequisites

Follow the instructions at [Getting Started](Getting_Started.md)

## Available Demos 

### Basics 

- [Basic calls to the ChatCompletion Endpoint](OpenAI/Basics/Prompt-basics.ipynb). Following scenarios included:
    
    1. Generate content 
    2. Summarizing
    3. Inferring 
    4. Transforming
    5. Expanding


- [Azure Function calling with Azure Open AI - Simple](OpenAI/Function-Calling-Simple/working_with_functions.ipynb) taken & modified from [repo](https://github.com/Azure-Samples/openai/tree/main/Basic_Samples/Functions)


### Intermediate
- TODO VECTOR Search basics based on https://gist.github.com/pablocastro/90677135ddbd1f8a4783006f6e890edf
      - VIDEO https://youtu.be/Xwx1DJ0OqCk 
- [Speech Summarizing with OpenAI and Azure Speech AI](OpenAI/Speech-Summarize/Speech-summarizing.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
- [Open AI and Azure Document Intelligence (Form Recognizer)](OpenAI/Document-Intelligence/Document-Intelligence.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)
    - Use Form Recognizer for Image to Text, and use "text-davinci" AOAI model to summarize.
- [Gradio webapp with Azure ChatGPT, your own chatGPT website](OpenAI/Gradio-ChatBot-WebApp/Gradio-WebApp-ChatGPT.ipynb) taken & modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)

- [Use OpenAI with your own data](OpenAI/OpenAI-YourData/README.md)

- [Azure Computer Vision and Langchain](OpenAI/ComputerVision-Langchain/computer-vision-langchain.ipynb) taken and modified from [repo](https://github.com/retkowsky/Azure-OpenAI-demos/)

- [Functions calling with Azure Open AI and Azure Search ]()  taken & modified from [repo](https://github.com/Azure-Samples/openai/tree/main/Basic_Samples/Functions)




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

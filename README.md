# Semantic Spotter Project Submission Report 
> To design and implement a robust Generative Search System for the insurance domain that leverages Retrieval-Augmented Generation (RAG) techniques to accurately and efficiently answer user queries based on diverse policy documents using LlamaIndex

## Table of Contents
* [General Info](#general-information)
* [Project Structure](#project-structure)
* [Business Context](#business-context)
* [Knowledge Base](#knowledge-base)
* [RAG pipeline building approach](#rag-pipeline-building-approach)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [How to run](#how-to-run)
  
## General Information
- For this assignment, a Python notebook containing RAG implementaion with Llamaindex framework is expected to submit
- This project aims to address issues with Insurance policy documents such as lengthy, complex, and difficult for users to interpret, leading to confusion and delays in decision-making.

## Project Structure
- `knowledge_base/`: Contains the pdf files that will be used for RAG.
- `api_key`: Contains OpenAI API key.
- `Semantic_Spotter_using_LlamaIndex_Submission_(F).ipynb`: Jupyter notebooks with Llamaindex RAG implementation.
- `Semantic_Spotter_using_LlamaIndex_Project_Report.pdf`: for detailed documentation.
- `README.md`: Project documentation and overview.

## Business Context
- In the insurance sector, policy documents are often dense, complex, and vary widely across products and providers.  
- This project aims to streamline access to critical information by building a generative search system powered by Retrieval-Augmented Generation (RAG). 
- By enabling accurate, context-aware responses to user queries, the solution enhances customer support, reduces manual effort, and improves decision-making for agents and policyholders alike.

## Knowledge Base
The following files are present inside knowledge_base folder. These files are provided by upGrad
- HDFC-Life-Easy-Health-101N110V03-Policy-Bond-Single-Pay.pdf
- HDFC-Life-Group-Poorna-Suraksha-101N137V02-Policy-Document.pdf
- HDFC-Life-Group-Term-Life-Policy.pdf
- HDFC-Life-Sampoorna-Jeevan-101N158V04-Policy-Document (1).pdf
- HDFC-Life-Sanchay-Plus-Life-Long-Income-Option-101N134V19-Policy-Document.pdf
- HDFC-Life-Smart-Pension-Plan-Policy-Document-Online.pdf
- HDFC-Surgicare-Plan-101N043V01.pdf
- Principal-Sample-Life-Insurance-Policy.pdf

## RAG pipeline building approach
> At high level this assignment is divided into following steps:
- Installing and implementing dependencies
- Creating common defitions for re-usability 
- Importing OpenAI API key 
- Loading all the documents from knowledge base for grounded truth
- Parsing all pdf files
- Creating nodes
- Bulding vector store and query
- Repeat the process with default values, chanding model and adding more specific settings
- Creating user interface with Gradio
- Submitting query and anlysising response with execution time

## How to run
For executing this RAG implementation, google colab is used because the environment setup becomes very easy with google colab. For any other execution environment such as windows machine, need to create requirements.txt with all technologies used.
Assuming this code will be directly executed with google colab, all the depencies are managed in the code file itself.
- upload 'Semantic_Spotter_using_LlamaIndex_Submission_(F).ipynb' to google colab.  
- Create a folder with name 'knowledge_base' and upload all the files.
- upload api_key.txt that contains OpenAI API key
- Click on 'Run All' (either from menu items Runtime->Run All or directly from Run All option
- monitor for any error
- Monitor responses of various queries (query_1 to query_8)
- Finally write query in Query section of Gradio and click on submit

## Conclusions
- LlamaIndex streamlines the creation of Retrieval-Augmented Generation systems by offering modular tools for document ingestion, indexing, and context-aware querying. 
- Its flexibility and integration with leading LLMs make it a powerful choice for building scalable, domain-specific search applications.


## Technologies Used
- Python - version 3.12.11
- PyMuPDF - version 1.26.4
- llama-index - version 0.14.3
- openai - version 1.109.1
- llama-index-core - version 0.14.3
- llama-index-embeddings-openai - version 0.5.1
- nest-asyncio - version 1.6.0
- ipython - version 7.34.0
- gradio - version 5.46.0
                           
## Acknowledgements
- Upgrad Team and instructors

## Contact
Created by [@GirishKolhe](https://github.com/GirishKolhe) - feel free to contact us!

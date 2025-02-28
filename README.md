# Local AI Agent with Qwen2.5 and LangChain Integration

## Overview

This project demonstrates how to deploy a private, local large language model (LLM), **Qwen2.5:1.5b**, using **Ollama** for local deployment. The project leverages the open-source framework **LangChain** for intelligent agent development, focusing on policy analysis tasks. 

By combining **Retrieval-Augmented Generation (RAG)** and local memory features, this solution addresses privacy concerns by processing sensitive data locally, making it ideal for government services, enterprise knowledge management, and digital platforms.

## Architecture

![Agent](https://github.com/user-attachments/assets/cb8ff27b-0ec4-4eca-86d0-bfdc2438a690)

The project architecture consists of the following components:
- **Local LLM Deployment**: We deploy **Qwen2.5:1.5b** locally using **Ollama** for private model inference.
- **LangChain Framework**: LangChain is used for local agent development, enabling structured output and API integrations.
- **Online Search Integration**: The **Zhipu AI** search engine API is used to enhance the agent’s capabilities with online search results.
- **Local Database**: User interactions are stored in an **SQL database** for memory persistence, enabling continuous conversations with the agent.

### Key Features
- **Policy Analysis Assistant**: The agent is designed using prompts to assist in policy analysis tasks.
- **Structured Output**: The agent generates structured outputs, such as formatted and segmented results, which can be used for various analysis and reporting tasks.
- **Local Memory**: The agent stores conversation history in a local database, allowing it to maintain a personalized and context-aware dialogue.
- **RAG Integration**: The system integrates the retrieval of online information using the Zhipu AI search API, enhancing the agent’s knowledge with relevant online data.

## Setup and Installation

### Prerequisites
Install **Miniconda** and set up your Python environment:
   ```bash
   conda create -n ollama-1 python=3.9
   conda activate ollama-1
   pip install ipykernel
   python -m ipykernel install --user --name ollama-1 --display-name ollama-1
   pip install -U langchain-ollama
   pip install zhipuai
   pip install langchain_community
   pip install langgraph
   pip install langgraph-checkpoint-sqlite==2.0.3
   pip install langgraph-prebuilt
   ```


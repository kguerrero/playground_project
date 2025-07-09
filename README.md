# A Little Inspirational Developer Helper: A RAG System

A playground space for familiarization with the latest RAG and agent libraries.  As well as a space to experiment with different LLM models and tokenization techniques

This repository sets up a local LLM (which can also be a call to the Hugging Face interface client), loads your favorite texts for guiding success as an engineer, and wraps everything into an RAG pipeline.

## base environment set up

```bash
conda create --name playground_project python=3.13
conda activate playground_project
pip install uv
```
    
## install dependencies

Navigate to the `playground_project` directory that contains the uv lock file and create a virtual environment.

```bash
uv sync
```

Note: You will need to authenticate to the Hugging Face community in the terminal if you want to use the remote inference API example. 

Recommended steps for authenticating to the server:
```
pip install -U "huggingface_hub[cli]"
huggingface-cli login
```

Reference websites for token setup: 
- https://huggingface.co/docs/hub/security-tokens
- https://huggingface.co/docs/huggingface_hub/main/en/guides/cli

## Overview

A FAISS index is used for storing context embeddings. The gemma3n model is the provided example of a locally running LLM.

```
curl -fsSL https://ollama.com/install.sh | sh

ollama pull gemma3n

ollama run gemma3n
```


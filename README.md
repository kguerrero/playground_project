# A Little Inspirational Developer Helper: A RAG System

A playground space for familiarization of latest RAG and agent libraries.  As well as a space to experiment with different LLM  models and tokenization techniques

This repository sets up a local LLM (can also be a call to hugging face interface client), loads in your favorite texts for guiding success as an engineer, and wraps everything into a RAG pipeline.

## base environment set up

```bash
conda create -- name playground_project python=3.13
conda activate playground_project
pip install uv
```
    
## install dependencies

navigate to `playground_project` directory that contains the uv lock file and create vertual environment

```bash
uv sync
```

Note: you will need to authenticate to the hugging face community in the terminal if you want to use the remote inference API example. 


## Overview

A FAISS index is used for storing context embeddings. The gemma3n model is the provided example of a locally running LLM.

```
curl -fsSL https://ollama.com/install.sh | sh

ollama pull gemma3n

ollama run gemma3n
```


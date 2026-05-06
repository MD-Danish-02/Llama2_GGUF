# Llama 2 & Perplexity AI Integration with LangChain in Google Colab

This project demonstrates how to work with both:

* Local/Open-Source LLMs using Hugging Face and Llama 2
* Cloud-based LLM APIs using Perplexity AI
* LangChain integration for prompt handling and LLM workflows
* Google Colab setup for running Generative AI experiments

The notebook covers model loading, inference, prompt engineering, and API integration workflows.

---

# Project Overview

In this project, I explored different ways of working with Large Language Models (LLMs).

The project includes:

* Llama 2 7B GGUF local inference
* Hugging Face Transformers integration
* LangChain integration
* Perplexity AI API integration
* Prompt engineering examples
* Google Colab setup
* API key management using Colab Secrets

---

# Technologies Used

* Python
* Google Colab
* Hugging Face Transformers
* LangChain
* LangChain OpenAI
* Llama.cpp
* Perplexity AI API
* OpenAI Compatible APIs
* PyTorch

---

# Features

## Local LLM Inference

* Load Llama 2 7B model locally
* Use GGUF models
* Run inference inside Google Colab
* Use Hugging Face pipelines

## Cloud LLM Integration

* Integrate Perplexity AI API
* Use Sonar model
* Connect LangChain with cloud APIs
* Secure API key handling using Colab Secrets

## Prompt Engineering

* System prompts
* Role-based prompting
* Beginner-friendly AI tutor prompts
* Technical assistant prompts

---

# Llama 2 Model Setup

The notebook includes:

* Loading tokenizer
* Loading model weights
* Using AutoModelForCausalLM
* Creating Transformers pipeline
* Generating AI responses

Example:

```python
model = "meta-llama/Llama-2-7b-chat-hf"
```

---

# Perplexity AI Integration

Perplexity AI was integrated using LangChain and OpenAI-compatible APIs.

Example:

```python
from langchain_openai import ChatOpenAI

llm = ChatOpenAI(
    api_key=os.environ["PPLX_API_KEY"],
    base_url="https://api.perplexity.ai",
    model="sonar"
)
```

---

# LangChain Integration

This project demonstrates how LangChain can be used with different LLM providers.

Implemented:

* ChatOpenAI wrapper
* invoke() method
* Prompt handling
* Response generation

---

# Google Colab Setup

The project is designed to run in Google Colab.

## Required Packages

```python
!pip install -q transformers
!pip install -q torch
!pip install -q langchain
!pip install -q langchain-openai
!pip install -q openai
```

---

# API Key Management

API keys were securely handled using Google Colab Secrets.

Example:

```python
from google.colab import userdata
import os

os.environ["PPLX_API_KEY"] = userdata.get("PPLX_API_KEY")
```

---

# Example Prompt

```python
response = llm.invoke(
    "Explain artificial intelligence in simple words."
)

print(response.content)
```

---

# Learning Outcomes

Through this project, I learned:

* Working with open-source LLMs
* Local model inference
* Cloud-based AI APIs
* LangChain integration
* Prompt engineering
* LLM workflows
* Colab-based AI development
* API handling and security

---

# Google Colab Notebook

Add your Google Colab notebook link here:

```text
[PASTE_YOUR_COLAB_NOTEBOOK_LINK_HERE](https://colab.research.google.com/drive/1e5vPF0n4WktP7qAzfvQNt45_xno4leua?usp=sharing)
```

Example:

```text
https://colab.research.google.com/drive/your_notebook_id
```

---

# GitHub Repository

Add your GitHub repository link here:

```text
[PASTE_YOUR_GITHUB_REPOSITORY_LINK_HERE](https://github.com/MD-Danish-02/Llama2_GGUF)
```

---

# Future Improvements

* Build AI chatbot
* Add Retrieval-Augmented Generation (RAG)
* Integrate vector databases
* Add memory functionality
* Create multi-agent workflows
* Build AI research assistant

---

# Author

Mohammad Danish Alam

Passionate about Artificial Intelligence, Generative AI, Automation, and LLM Engineering.

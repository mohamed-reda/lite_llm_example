# LiteLLM Google Colab Integration

This project demonstrates how to integrate LiteLLM, a lightweight and open-source library for managing Large Language
Models (LLMs), within a Google Colab environment. It showcases various features of LiteLLM, including proxy server
setup, load balancing, fallbacks, and observability.

## Features

* **Proxy Server:** Sets up a local proxy server using LiteLLM to route requests to different LLMs, allowing you to use
  the OpenAI API or LangChain to interact with LLMs hosted by LiteLLM.
* **Load Balancing:** Configures load balancing with LiteLLM to distribute requests across multiple LLMs for improved
  performance and reliability.
* **Fallbacks:** Implements fallbacks to automatically switch to a different LLM if the primary one is unavailable or
  fails to respond.
* **Observability:** Integrates with LangFuse to monitor and track LLM usage and performance.
* **LangChain Integration:** Demonstrates how to use LiteLLM with LangChain for tasks such as summarizing web page
  content.

## Requirements

* **Google Colab:** A Google Colab notebook to run the code.
* **LiteLLM:** Install using `!pip install 'litellm[all]'`.
* **LangChain:** Install using `!pip install -qU langchain-openai langchain langchain_community transformers`.
* **API Keys:** Set the following environment variables with your API keys:
    * `GOOGLE_API_KEY`
    * `GEMINI_API_KEY`
    * `COHERE_API_KEY`
    * `GROQ_API_KEY`
    * `LANGFUSE_PUBLIC_KEY`
    * `LANGFUSE_SECRET_KEY`
    * `HUGGINGFACE_API_KEY`

## Usage

1. **Clone this repository or copy the code into a Google Colab notebook.**
2. **Install the necessary libraries.**
3. **Set the environment variables.**
4. **Run the code cells in the notebook.**

## Examples

The notebook provides various examples of using LiteLLM with different LLMs, such as:

* Calling Cohere's command-r-plus-08-2024 model.
* Calling Google's Gemini Pro model.
* Using proxy server with Groq models, gemma2-9b-it and mixtral-8x7b-32768.
* Using load balancer to distribute load across multiple models.
* Using fallbacks to switch to alternative models in case of failure.
* Integrating with LangFuse to monitor LLM performance.
* Using LiteLLM and LangChain together to chain LLMs or using langchain modules like summarization.

## Disclaimer

This project is for educational and demonstration purposes only. Google Colab instances are temporary and may be
terminated, resulting in data loss.

## Acknowledgements

* **LiteLLM:** [LiteLLM](https://github.com/BerriAI/litellm) project for providing the LLM management library.
* **LangChain:** [LangChain](https://github.com/langchain-ai/langchain) project for facilitating interaction with LLMs.
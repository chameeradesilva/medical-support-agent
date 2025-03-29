# medical-support-agent

This repository contains a Google Colab notebook that implements a simplified medical coding and diagnosis system using open-source Large Language Models (LLMs). The system simulates a multi-agent workflow where different virtual medical specialists collaborate to diagnose a patient based on provided symptoms and suggest treatment plans.

## Overview

The system consists of the following key components:

* **Agents:** Virtual medical specialists (e.g., Medical Coder, Diagnostic Synthesizer, Treatment Agent) each with a specific role and system prompt.
* **LLM:** An open-source LLM from Hugging Face Transformers (`google/flan-t5-base` by default) is used to power the agents.
* **Workflow:** The agents are executed sequentially, with the output of one agent serving as the input for the next.
* **Output:** The final output is a structured report in JSON format containing the outputs from each agent and a summary.

**Note:** This project is a simplified implementation and is intended for educational and experimental purposes. The accuracy and reliability of the diagnoses and treatment suggestions are subject to the capabilities of the chosen open-source LLM.

## Future Enhancements

Future development plans for this project include:

* Implementing a more advanced agentic framework to enable more complex interactions and collaboration between agents.
* Integrating vector databases to store and retrieve relevant medical knowledge, allowing for better Retrieval-Augmented Generation (RAG) and improved accuracy in diagnoses and treatment suggestions.

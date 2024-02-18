---
layout: post
title: "Open Source Projects that use AUTOGEN"
date: 2024-02-18
categories: AI releases
---

### AutoGen AGI
- **Developer:** [GitHub Username]
- **URL:** [AutoGen AGI](https://github.com/[username]/AutoGenAGI)
- **Description:** This project aims at advancing AI agents towards AGI capabilities using AutoGen, focusing on group chat dynamics, decision-making, and complex task proficiency.

### Promptulate
- **Developer:** Undertone0809
- **URL:** [Promptulate](https://github.com/Undertone0809/promptulate)
- **Description:** A framework for LLM automation and autonomous language agents development, enabling the creation of LLM Agent Applications in a pythonic way.

### Generative AI Workbook
- **Developer:** AaronWard
- **URL:** [Generative AI Workbook](https://github.com/AaronWard/generative-ai-workbook)
- **Description:** Serves as a central repository for all LLM development, containing various projects and experiments utilizing AutoGen.

### AutoGenLabs
- **Developer:** radman-x
- **URL:** [AutoGenLabs](https://github.com/radman-x/AutoGenLabs)
- **Description:** Provides components and experiments to assist AutoGen developers, focusing on enhancing the capabilities of LLM applications.

### Roq-Scripts
- **Developer:** roq-trading
- **URL:** [Roq-Scripts](https://github.com/roq-trading/roq-scripts)
- **Description:** Features scripts for setting up development environments, auto-generating C++ code, and more, leveraging AutoGen for efficiency.

### Agent Adapters
- **Developer:** nalbion
- **URL:** [Agent Adapters](https://github.com/nalbion/agent-adapters)
- **Description:** A configurable framework for AI Agents that facilitates a variety of configurations and integrations with AutoGen.

### AgentCloud
- **Developer:** rnadigital
- **URL:** [AgentCloud](https://github.com/rnadigital/agentcloud)
- **Description:** Combines Python and Next.js to feature an autogen-enabled agent backend and a web app, streamlining workflows with AutoGen.

### AI Repository by TylerProgramming
- **Developer:** tylerprogramming
- **URL:** [AI Repository by TylerProgramming](https://github.com/tylerprogramming/ai)
- **Description:** Hosts various projects using AutoGen, along with tutorials to facilitate learning and development in the domain of LLM.

### Chainlit-AutoGen
- **Developer:** AaronWard
- **URL:** [Chainlit-AutoGen](https://github.com/AaronWard/generative-ai-workbook/blob/main/personal_projects/9.chainlit-autogen/README.md)
- **Description:** Integrates Chainlit with AutoGen to enhance project development capabilities in LLM applications.

### DivyaKandeepan's AutoGen Projects
- **Developer:** DivyaKandeepan
- **URL:** [DivyaKandeepan's AutoGen Projects](https://github.com/DivyaKandeepan/Autogen_projects)
- **Description:** Includes a collection of projects that utilize AutoGen for developing LLM applications, though specific project details are not provided.

### Task Tree Agent
- **Developer:** SuperpoweredAI
- **URL:** [Task Tree Agent](https://github.com/SuperpoweredAI/task-tree-agent)
- **Description:** Utilizes GPT-4 for building an LLM-powered autonomous agent capable of hierarchical task management. Introduces a dynamic tree structure for task organization.


# What is AUTOGEN?

## Introduction

AutoGen is a groundbreaking framework developed by Microsoft, focusing on the development of Large Language Model (LLM) applications through multi-agent conversations. This framework allows for the integration of customizable, conversable agents that can operate using a mix of LLMs, human inputs, and tools to solve complex tasks. The project represents a significant step forward in the automation and optimization of complex LLM workflows, demonstrating the potential for diverse application domains and conversation patterns.

## Project URL

For more details, visit AutoGen's main repository and documentation:
- GitHub Repository: [https://github.com/microsoft/autogen](https://github.com/microsoft/autogen)
- Documentation and Guides: [https://microsoft.github.io/autogen](https://microsoft.github.io/autogen)

## Key Features

- **Multi-Agent Conversations:** Enables building next-gen LLM applications by simplifying the orchestration, automation, and optimization of complex LLM workflows.
- **Customizable and Conversable Agents:** Offers a wide range of conversation patterns and the integration of LLMs, tools, and human inputs.
- **Enhanced LLM Inference:** Provides advanced features like API unification, caching, error handling, and multi-config inference.

## Latest Breakthroughs

- **Project Genesis:** AutoGen was first created in FLAML and later spun off as its own project, reflecting its significant evolution and the ongoing collaboration between Microsoft, Penn State University, and the University of Washington.
- **Cutting-Edge Applications:** The framework has been utilized to demonstrate a wide range of applications, from automated chess playing to supply chain optimization, showcasing its versatility and effectiveness in reducing coding effort and manual interactions.

## Code Examples and Use Cases

AutoGen's versatility is highlighted through various use cases and examples provided in its documentation. These include automated code generation, task solving with coding and planning agents, multimodal agent chats, and even playing chess with GPT-4 agents. It supports applications like web search, SQL query generation from natural language, and automated continual learning from new data.

## Installation and Getting Started

AutoGen requires Python version >= 3.8, < 3.11, and can be installed using pip. It is recommended to use Docker for code execution. A quick start involves cloning the repository, setting up LLM inference endpoints, and starting with the provided notebooks.

```bash
pip install pyautogen
```


```python
from autogen import oai

# Assuming you've set up your local LLM server with Ollama and have the endpoint ready
# Here's how you might interact with it using AutoGen's oai.Completion

response = oai.Completion.create(
    config_list=[
        {
            "model": "ollama-model-name",  # Specify your Ollama model name here
            "base_url": "http://localhost:8000/v1",  # This should point to your local Ollama server
            "api_type": "openai",
            "api_key": "NULL",  # Placeholder, not required for local servers
        }
    ],
    prompt="Hi",
)
print(response)

# For chat completion with Ollama
response = oai.ChatCompletion.create(
    config_list=[
        {
            "model": "ollama-model-name",  # Again, specify your Ollama model
            "base_url": "http://localhost:8000/v1",  # Local Ollama endpoint
            "api_type": "openai",
            "api_key": "NULL",
        }
    ],
    messages=[{"role": "user", "content": "Hi"}]
)
print(response)
```


This code snippet shows how to configure AutoGen to communicate with a locally hosted LLM, such as Ollama, using FastChat as a local server that provides OpenAI-compatible APIs. While this example is not directly from the search results, it's inspired by the process described in the AutoGen documentation for local LLM applications. Adjustments may be needed to align with specific requirements or configurations of the Ollama model you intend to use.

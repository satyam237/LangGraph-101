# LangGraph Concepts & Beginner Codes Notebook

This repository contains a Jupyter Notebook where I document my journey into understanding LangGraph—a framework for building stateful, multi-agent applications with language models. The notebook covers key concepts, beginner-level code examples, and practical experiments.

<details>
Table of Contents
Overview
[Part 1: Getting Started]
[Part 2: Adding Tools]
[Part 3: Adding Memory]
[Part 4: Human-in-the-Loop]
[Part 5: Customizing Graph State]
[Part 6: Time Travel]

</details>
  
References & Further Reading
How to Run
Contributing
License
Overview
This notebook serves as a hands-on guide for beginners to learn how LangGraph works. Inspired by the official LangGraph tutorials, it explores the following topics:

Building an LLM application using Groq's LLM models.
Integrating external tools (like the Tavily search tool) to enhance chatbot capabilities.
Enabling persistent memory via checkpointing to support multi-turn conversations.
Incorporating human oversight in the execution loop (human-in-the-loop).
Customizing and extending the state schema for advanced workflows.
Implementing time travel to rewind or branch conversation history.

## Part 1: Getting Started
Topic: Creating a basic LLM application.
Focus: Use Groq's LLM models to build a simple chatbot.
Objective: Learn how to initialize a state graph, add nodes and edges, and compile the graph.

## Part 2: Adding Tools
Topic: Enhancing chatbot functionality.
Focus: Integrate external tools—specifically, a search tool (Tavily)—to answer queries beyond the chatbot's built-in knowledge.
Objective: Understand how to bind tools to the LLM and invoke them within the graph.

## Part 3: Adding Memory
Topic: Persistent conversation state.
Focus: Utilize checkpointing so that the chatbot can remember past interactions.
Objective: Enable multi-turn conversations with coherent context across sessions.

## Part 4: Human-in-the-Loop
Topic: Incorporating human oversight.
Focus: Allow interruptions in the automated process for human review or confirmation.
Objective: Build a chatbot that can pause execution, await human input, and then resume processing.

## Part 5: Customizing Graph State
Topic: Extending the state schema.
Focus: Add additional keys (such as user details or custom variables) to the graph state.
Objective: Learn how to customize state handling to support more complex workflows.

## Part 6: Time Travel
Topic: Rewinding and branching conversation history.
Focus: Use checkpointing to "rewind" to previous states and explore alternative conversation paths.
Objective: Implement time travel capabilities for debugging, experimentation, or alternative decision paths.
References & Further Reading
For more detailed information and official guidance, please refer to the LangGraph tutorials.

How to Run
Clone the Repository:

```bash
git clone https://github.com/your_username/your_repo_name.git
cd your_repo_name
```

Install Required Packages:

Make sure you have Python installed, then run:

```bash
pip install -U langgraph langsmith langchain_anthropic tavily-python
```

Set Up API Keys:

The notebook requires API keys (e.g., for Anthropic and Tavily). The code includes a helper function to prompt for these if they are not already set in your environment.

Run the Notebook:

Open the Jupyter Notebook (e.g., using Jupyter Lab or Notebook) and execute the cells sequentially.

Contributing
Contributions, feedback, and suggestions are welcome! Please feel free to open an issue or submit a pull request.

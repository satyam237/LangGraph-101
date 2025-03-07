<br>

# Getting Started with LangGraph: Concepts & Code

This repository contains a Jupyter Notebook documenting my journey into LangGraph—a framework for building stateful, multi-agent applications with language models. It includes key concepts, beginner-level code examples, and practical experiments, utilizing **Groq's Free API** for various available models.

<br>

## **Table of Contents**

- [**Overview**](#overview)
- [**Part 1: Getting Started**](#part-1-getting-started)
- [**Part 2: Adding Tools**](#part-2-adding-tools)
- [**Part 3: Adding Memory**](#part-3-adding-memory)
- [**Part 4: Human-in-the-Loop**](#part-4-human-in-the-loop)
- [**Part 5: Customizing Graph State**](#part-5-customizing-graph-state)
- [**Part 6: Time Travel**](#part-6-time-travel)
- [**References & Further Reading**](#references--further-reading)
- [**How to Run**](#how-to-run)
- [**Contributing**](#contributing)
- [**License**](#license)


<br>

## **Overview**
This notebook serves as a hands-on guide for beginners to learn how LangGraph works. Inspired by the official LangGraph tutorials, it explores the following topics:

- Building an LLM application using Groq's (free) LLM models.
- Integrating external tools (like the Tavily search tool) to enhance chatbot capabilities.
- Enabling persistent memory via checkpointing to support multi-turn conversations.
- Incorporating human oversight in the execution loop (human-in-the-loop).
- Customizing and extending the state schema for advanced workflows.
- Implementing time travel to rewind or branch conversation history.
<br>

## **Part 1: Getting Started**
Learn how to initialize a StateGraph, add nodes and edges, and compile your graph to create a basic chatbot.<br>
*Detailed code and explanations are provided in the notebook.*


## **Part 2: Adding Tools**
Enhance the chatbot by binding external tools (like the Tavily search engine) to your LLM. This enables the chatbot to answer queries beyond its built-in knowledge.


## **Part 3: Adding Memory**
Implement persistent checkpointing so that the chatbot remembers past interactions, enabling coherent multi-turn conversations.


## **Part 4: Human-in-the-Loop**
Incorporate human oversight into your workflow. The chatbot can pause execution for manual review or confirmation before resuming.<br>
_Build a chatbot that can pause execution, await human input, and then resume processing._


## **Part 5: Customizing Graph State**
Customize and extend the state schema to include additional information (e.g., user details) to support more complex application logic.<br>
_Learn how to customize state handling to support more complex workflows._


## **Part 6: Time Travel**
Implement time travel functionality to rewind to previous conversation states or branch off new execution paths for debugging and experimentation. <br>
*Use checkpointing to "rewind" to previous states and explore alternative conversation paths.*

<br>

## **References & Further Reading**
For more detailed information and official guidance, please refer to the [LangGraph tutorials.](https://langchain-ai.github.io/langgraph/tutorials/introduction/)


<br>

## **How to Run**
1. Clone the Repository:

Navigate to the Desired Directory
```bash
cd /path/to/your/directory
```

Clone the Repository using https:
```bash
git clone https://github.com/satyam237/LangGraph-Concepts-Notebook.git
```

Enter the Cloned Repository
```bash
cd repo
```

2. Install Required Packages:

  Make sure you have the `requirements.txt` and `Python3.10` or above installed, then run:

```bash
pip install -r requirements.txt
```

3. Set Up API Keys:

  The notebook requires API keys (e.g., for Groq/Anthropic and Tavily). The code includes a helper function to prompt for these if they are not already set in your environment.
  Create an account on each of these website and generate the API key, and store it in `.env` file, and use `loadenv()` to call them, as given in the notebook:
  
  ```bash
  GROQ_API_KEY="YOUR_API_KEY_HERE"
  TAVILY_API_KEY="TAVILY_API_KEY_HERE"
  ```
  
  or you can also store them as environment variable on the local machine itself:

  ```bash
  export GROQ_API_KEY="API_KEY"
  ```
  same way,do for all other keys, and use the function at the very start to call these keys. (*this function also helps store the key as we go without storing it anywhere.*)
  

4. Run the Notebook:

  Open the Jupyter Notebook (e.g., using Jupyter Lab or Notebook) and execute the cells sequentially.

<br>

## **Contributing**
 Contributions, feedback, and suggestions are welcome! Please feel free to open an issue or submit a pull request.

<br>


## License

This project is licensed under the terms of the [MIT license](https://github.com/satyam237/LangGraph-Concepts-Notebook/tree/main?tab=MIT-1-ov-file).

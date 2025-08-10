# ReAct Implementation from Scratch with LangChain

This project demonstrates a custom implementation of the **ReAct** (Reason + Act) pattern using [LangChain](https://www.langchain.com/).  
Instead of relying on a prebuilt LangChain agent, the reasoning loop and tool execution are implemented manually to better understand how the ReAct framework works.

## How It Works
The **ReAct** pattern allows a language model to:
1. **Reason** about a problem (generate thoughts).
2. **Act** by calling tools to gather information.
3. Repeat the Reason → Act cycle until it reaches the final answer.

In this project:
- We define a single tool: `get_text_length` – returns the length of a string.
- The LLM (Ollama's `llama3` model) is prompted with a custom ReAct-style template.
- The script parses LLM output, determines whether to take an action or finish, executes the action if needed, and loops until a final answer is reached.
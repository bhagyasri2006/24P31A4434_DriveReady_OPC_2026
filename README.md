# AgenticAI

# Day 1 – AI Customer Complaint Classifier
This project introduces the use of Large Language Models (LLMs) to analyze and classify customer complaints. The system accepts complaints written in natural language and automatically identifies the main issue, its priority, and the reason for classification.
## Objective
The objective is to build a basic AI-powered complaint classification system that reduces the need for manual complaint categorization and helps customer support understand customer issues more efficiently.
## Concepts Learned
- Introduction to Large Language Models (LLMs)
- Connecting Python applications with AI models
- Prompt engineering and system prompts
- Natural language processing using an LLM
- Complaint categorization and priority identification
## Implementation
The application uses Python and the Groq API to communicate with a language model. A system prompt defines the role of the AI as a customer complaint classification assistant. The model analyzes the complaint and identifies its category, priority, and reason.
## Technologies Used
- Python, Groq API, LangChain / ChatGroq ,Jupyter Notebook
## Outcome
A working AI complaint classifier was developed that can analyze customer complaints and generate structured classification results. This project forms the foundation for adding advanced features such as memory, testing, and AI agent tools in subsequent days.



# Day 2 – Advanced Complaint Classification
Day 2 extends the basic complaint classifier by improving its response consistency, structure, and error handling. The system is designed to produce more organized results and handle different complaint scenarios effectively.
## Objective
The objective is to improve the AI complaint classifier using advanced prompting techniques, structured outputs, reusable functions, and basic error-handling mechanisms.
## Concepts Learned
- System prompting and few-shot prompting
- Structured JSON output generation
- Python dictionaries and functions
- Decorators and function wrapping
- Exception handling
- Basic conversational memory
## Implementation
-A detailed system prompt is used to define the classification rules and available complaint categories. Few-shot examples help the model understand the expected format and behavior. The model returns complaint information in JSON format, including category, priority, and reason.
-Python functions are used to organize the classification logic. Decorators demonstrate function behavior and logging, while exception handling helps manage unexpected errors. A basic memory mechanism is also implemented to maintain conversational context.
## Technologies Used
- Python, Groq API,LangChain,JSON,Jupyter Notebook
## Outcome
The classifier was tested with multiple complaint examples, including payment issues, delayed deliveries, damaged products, refund problems, and login difficulties. The implementation improved the organization, reliability, and maintainability of the complaint classification system.



# Day 3 – LangChain and AI Agent Introduction
## Project Overview
Day 3 focuses on integrating the customer complaint classifier with LangChain. The project moves beyond a simple LLM call and introduces prompt templates, chains, conversational memory, testing, and the basic architecture of AI agents.
## Objective
The objective is to understand how LangChain simplifies the interaction between prompts and language models and how an AI agent can be designed to perform tasks using tools.
## Concepts Learned
- Chatbots versus AI agents
- Components of an AI agent
- Agent execution loop: Think, Act, Observe, and Repeat
- Prompt templates and message placeholders
- LangChain chains
- Conversation memory
- Testing with CSV datasets
- Temperature and model response variation
## Implementation
-The complaint classifier is connected to Groq using ChatGroq. ChatPromptTemplate is used to create reusable prompts, while MessagesPlaceholder supports conversational context. A chain connects the prompt, language model, and output parser.
-A separate complaint testing dataset is created to evaluate the classifier against different complaint categories. The create_agent framework is also explored to understand the basic structure of an AI agent.
## Technologies Used
- Python,LangChain,LangChain-Groq,Groq API,CSV,Jupyter Notebook
## Outcome
The project now uses LangChain components for prompt management, model interaction, and conversation context. It also introduces the foundation for an AI agent that can use tools to perform additional tasks instead of only generating text.



# Day 4 – Tool-Enabled Customer Complaint Agent
## Project Overview
Day 4 extends the complaint classification project into a tool-enabled AI agent. The agent is designed to analyze customer complaints, access category information, suggest priorities, and save complaint records when requested.
## Objective
The objective is to understand how AI agents interact with tools and how tool functions can extend the capabilities of a language model beyond text generation.
## Concepts Learned
- AI agents and tool calling
- Creating tools using the LangChain tool decorator
- Tool descriptions and arguments
- Connecting multiple tools to an agent
- Agent decision-making and tool selection
- Complaint logging and CSV file handling
- Conversational interaction with an agent
## Implementation
-The agent is designed with three tools: get_category_info, suggest_priority, and log_complaint. The category information tool provides details about complaint categories, while the priority tool suggests a default priority for a given category.
-The complaint logging tool stores complaint information in a CSV file, including timestamp, complaint text, category, priority, sentiment, reason, and recommended action. The agent is connected to these tools using LangChain's create_agent framework.
## Technologies Used
- Python,LangChain,LangChain-Groq,Groq API,CSV,Pydantic
## Outcome
The project is extended toward a tool-enabled customer complaint agent that can use Python functions for additional tasks. It demonstrates the difference between a basic chatbot and an AI agent capable of interacting with tools. The implementation can be further improved with validation, testing, and additional customer support tools.

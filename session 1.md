# **🚀 Session 1: Introduction to LLMs and APIs**

## **🎯 Objective**

By the end of this session, students will:

- ✅ Understand how to call an LLM via an API using Groq.
- ✅ Send basic prompts and process responses using LangGraph.
- ✅ Begin brainstorming their final project workflow using LangGraph.

---

## **1️⃣ Calling an LLM via API**

### **🧐 Understanding API-Based LLMs**

Unlike running an LLM on a local machine, we will interact with the model through an API. The API processes a request, generates a response, and returns it. This method is efficient and offloads computational complexity to external servers.

### **⚙️ Setting Up**

Before using LangGraph to call an LLM, ensure you have the following:

- 🐍 New virtual environment (see previous documents)
- 📦 `langgraph` and `groq` installed via pip:
    
    ```bash
    pip install langgraph langchain-openai langchain
    ```
    
- 🔑 An API key for Groq.
- Setup the config file, fill in `your key` (keep it secret):
```python
# from langchain_groq import ChatGroq
# import os

# # Set up API key
# os.environ["GROQ_API_KEY"] = "your key"
# llm = ChatGroq(model="llama-3.1-8b-instant")

from langchain_openai import ChatOpenAI
import os

llm = ChatOpenAI(
    api_key="your key",
    base_url="https://dashscope.aliyuncs.com/compatible-mode/v1",
    model="qwen-turbo",
    # other params...
)
```

> you can also use other llms as long as they support langchain/langgraph (search on the Internet)

### **📝 Basic Example: Calling an LLM in LangGraph**

Here’s a simple script to send a prompt and get a response:

```python
# a seperate file from config.py, make sure they are under the same directory
import os
from config import llm

# Invoke the model with a prompt
response = llm.invoke("What is LangGraph?")

print(response)
```

### **💡 Hands-On Activity: Send Your Own Prompt**

#### **🟢 Easy Challenge:**

- Modify the script to accept user input from the command line and pass it to the model.
    
    ```python
    user_prompt = input("Enter your prompt: ")
    response = llm.invoke(user_prompt)
    print("Response:", response)
    ```
    

#### **🔴 Pro Challenge:**

- 🤖 Build an assistant with conversation memory.
- 🗂️ Use a dictionary or a simple database to store past interactions.
- 🔄 Modify the script to consider previous responses when generating new ones.

---

## **2️⃣ Final Project Brainstorm: Designing a Custom Workflow**

### **🧠 Overview**

Since this course is about building workflows using LangGraph, students should start thinking about the kind of project they want to build.

### **❓ Guiding Questions**

- 🤔 What type of workflow do you want to automate using an LLM?
- 🔄 Will your project involve multi-step interactions?
- 🌐 Do you want it to fetch external information (e.g., Wikipedia, APIs)?
- 🏗️ Will it involve user personalization?

### **✍️ Hands-On Activity: Idea Sketching**

#### **📌 Task:**

- Spend 5-10 minutes sketching a simple workflow idea on paper or in a text editor.
- Identify at least two key interactions the user will have with the system.
- Share ideas with a partner or the group for feedback.

#### **🟢 Easy Challenge:**

- 📝 Define the input and output of your workflow clearly.
- 🔀 Identify one decision point in your workflow (e.g., user response changes the next step).

#### **🔴 Pro Challenge:**

- 📊 Create a simple flowchart of your workflow idea.
- 🔗 Identify at least one external tool or API you may want to integrate.
- 🛠️ Consider an optional advanced feature (e.g., memory to track user progress).

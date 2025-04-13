# **Session 3: Enhancing LLM Responses with External Tool Integrations in prompts, an Intro** 🚀

## **Objective** 🎯

By the end of this session, students will:

- Understand how integrating external tools can make LLM responses more accurate and engaging. 🔧
- Explore **Prompt-Based Integration:** Example of Augmenting prompts with externally retrieved data using RAG.
- Gain hands-on experience through live demonstrations and group activities. 💻

---

## **1. Introduction to External Tool Integrations** 🔍

### **Why Integrate External Tools?** 🤔

- **Enhanced Accuracy & Relevance:**  
    Including real-time data or specialized functions can tailor responses to specific needs.
- **Dynamic Functionality:**  
    The LLM can execute tasks (like API calls or computations) that go beyond its training data.
- **Real-World Applications:**  
    From fact-checking with RAG to executing calculations with LangChain tools, these integrations empower versatile solutions.

![[/_resources/Pasted image 20250308225059.png]]

> official document: https://python.langchain.com/docs/concepts/tool_calling/

---

## **2. Integration Methods Overview** 🛠️

### **Example: Prompt-Based Integration (RAG)** 🔄

Example code: https://github.com/Computing-Society-CSC/LangGraph_Examples2025

- **Concept:**  
    Retrieval-Augmented Generation (RAG) enriches LLM prompts with data fetched from external sources.
- **How It Works:**
    1. Query an external data source (e.g., an API or database).
    2. Embed the retrieved information into the prompt.
    3. Let the LLM generate responses using this added context.
- **Example Scenario:**  
    Imagine augmenting a prompt with up-to-date weather data to provide accurate travel advice. 🌤️

---

## **3. Demonstrations and Hands-On Activities** 🎥🕹️

### **Live Demonstration: Prompt-Based Integration** 💡

#### **Steps:**

1. **Show a Code Example:**
    - Demonstrate how to fetch external data (e.g., a simple API call).
    - Illustrate how to embed this data into the prompt for the LLM.
2. **Discuss the Benefits & Challenges:**
    - **Pros:** Enhanced context, improved factual accuracy.
    - **Cons:** Prompt length limits, manual orchestration of data fetching.


---


### **Instructions:**

Enhance a base LLM prompt with an external API (RAG approach).
- **Mini-Project:**  
    Build a mini-project where the LLM uses the chosen method to provide enhanced responses. For example, integrate a simple API to retrieve fun facts or current events. 🌐
    

### **Guiding Questions:**

- How does integrating external data change the quality of the response?
- What are some real-world applications where this integration would be useful?

### **Some Resources**


select a free api from here: https://github.com/public-apis/public-apis

create a workflow that makes llm use an external api.


Here's a prompt you can use to generate code that calls a certain API, based on the structure you've provided:

---

**Prompt:**

"Given the following API document, generate Python code that calls the specified API and logs the returned data to the console in a structured format:

API Document Example:

- Endpoint: `https://animechan.io/api/v1/quotes/random`
- Response:

```json
{
    "status": "success",
    "data": {
        "content": "The final door is about to open! And I am the one opening it! Then the world that we know of will come to an end! This world of insatiable desires will end!",
        "anime": {
            "id": 575,
            "name": "Mobile Suit Gundam SEED",
            "altName": "Kidou Senshi Gundam SEED"
        },
        "character": {
            "id": 1486,
            "name": "Rau Le Creuset"
        }
    }
}
```

Your task is to create a fetch request to this API, and output the data's content, anime name, and character name in a readable format, similar to:

`Character: Rau Le Creuset, from the anime Mobile Suit Gundam SEED, said: "The final door is about to open! And I am the one opening it!"`

Generate the Python code below:"

---

This prompt instructs the model to generate code that handles the API call and displays the relevant data according to the structure in the document.


---

## **5. Wrap-Up and Q&A** 📝

- **Summary:**  
    Recap the key points on how both integration methods work and when to use each.
- **Discussion:**  
    Encourage students to share their group experiences and any challenges they encountered.
- **Q&A Session:**  
    Open the floor for questions, clarifications, and suggestions.

---

## **Additional Resources** 📚

- **Documentation:**
    - [LangChain Official Docs](https://langchain.readthedocs.io/)
    - Tutorials on RAG and external API integration.
- **GitHub Repository:**  
    A shared repository with sample projects and code snippets for both integration methods.
- **Further Reading:**  
    Articles and videos on best practices for LLM integrations.

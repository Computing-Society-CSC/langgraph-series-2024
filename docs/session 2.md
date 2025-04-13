# **Session 2: Diving Into LangGraph and Graph Traversal** 🧑‍💻

## **Objective** 🎯

By the end of this session, students will:

- Understand basic graph concepts and traversal methods. 🔍
- Be able to define and use **StateGraph** in LangGraph. 🔄
- Practice describing graph traversal using natural language or pseudocode. ✍️

---

## **1. Introduction to Graphs** 📊

### **Graph Representation in Computer Science** 🌐

- **What is a Graph?**  
    A **graph** is made up of **nodes** (vertices) and **edges** (connections between nodes).
    - **Nodes** represent entities like people, cities, or concepts. 🌍
    - **Edges** represent relationships or connections between nodes. 🔗

### **Key Graph Concepts** 🔑

- **In-degree (入度)**: The number of **incoming** edges to a node. ⬇️
- **Out-degree (出度)**: The number of **outgoing** edges from a node. ⬆️

---

## **2. Activity: Exploring Graph Concepts** 🕹️

### **Task 1: Representing Graphs** ✏️

#### **Instructions**:

Describe a graph using the following concepts:

- **Example:** "Describe a social network of Computing Society. Each person is connected to others with one-way relationships (e.g., Alice follows Bob, Bob follows Charlie, etc.)."
    
    - How would you define the graph using nodes and edges? 🤔
    - What are the **in-degrees** and **out-degrees** of each node?


---

### **Task 2: Graph Traversal (Natural Language / Pseudocode)** 🤖

#### **Instructions**:

Instead of coding, you will describe or write pseudocode for graph traversal algorithms. 📝

- **Breadth-First Search (BFS) – Natural Language Description** 🌊:
    
    - **Activity:** Describe how **BFS** works in simple terms:
        - "Imagine you are exploring a maze where you are standing at the entrance (node). BFS would ==explore all the rooms (nodes) that are one step away first==, before moving to the rooms that are two steps away, and so on." 🏰
        - Describe how BFS would work on a small network (e.g., a family tree or a simple social network). 👨‍👩‍👧‍👦
- **Depth-First Search (DFS) – Natural Language Description** ⛏️:
    
    - **Activity:** Describe how **DFS** works in simple terms:
        - "Imagine you are walking down a path in a forest, and whenever you find a fork in the road, you always take the first path you see. You ==continue down that path until you hit a dead end, then go back== to the last fork and try a different path." 🌲
        - Describe how DFS would work in a network or graph of your choice (e.g., a series of connected rooms in a house). 🏡

---

## **3. Hands-On Activity: Building a Simple StateGraph in LangGraph** ⚙️

### **What is LangGraph's StateGraph?** 🧠

- **StateGraph** is a core concept in LangGraph that helps define workflows and manage states. 

### **Creating Your First StateGraph**:

#### **Instructions**:

- Define a simple workflow using LangGraph's **StateGraph**:
    - Example: A basic conversation flow where the assistant asks for the user's name, then asks if they'd like to know the weather. 🌤️

see example project: https://github.com/Computing-Society-CSC/dual_hearts_roleplay


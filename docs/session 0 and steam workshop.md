# **How to Play with GPTs?**

_Introduction to Prompt Engineering for Instruction-Tuned LLMs_

## **Workshop Overview**

### ⏰ Estimated Duration: 1 Hour

### 🎯 Objectives:

- 🌟 Understand instruction-tuned LLMs and their capabilities.
- ✍️ Apply principles and tactics to create effective prompts.
- 🔍 Explore advanced techniques like summarization and prompt iteration.

---

## **1. Introduction to LLMs** (10 Minutes)

### 🤖 **Base LLMs vs. Instruction-Tuned LLMs**

- **Base LLMs**:  
    Trained on general data, excelling at tasks like predicting the next word based on context. They are less effective for task-specific or instruction-following use cases.
- **Instruction-Tuned LLMs**:  
    Optimized through Reinforcement Learning with Human Feedback (RLHF), enabling them to respond more accurately to direct instructions.


![[/_resources/Pasted image 20241209212959.png]]

> Further reading about the concepts: [The simple explanation of ChatGPT (LLM+RLHF) using Shoggoth with Smiley Face meme🙂🙂🙂 | by Deividas Mataciunas | Medium](https://medium.com/@mataciunasdeividas/the-simple-explanation-of-chatgpt-llm-rlhf-using-shoggoth-with-smiley-face-meme-947a0e9fb441)

### 📌 Examples:

**Base LLM Example:**

```markdown
Prompt: "Once upon a time, a brave knight embarked on a quest to save..."  
Output:  
"...the princess from a fierce dragon guarding a mysterious treasure."  
```

**Instruction-Tuned LLM Example:**

```markdown
Prompt: "Write a brief story about a brave knight saving a princess, keeping the tone lighthearted and including a talking dragon."  
Output:  
"Once upon a time, a brave knight named Sir Chuckles set out to save Princess Laughter from a mischievous dragon named Giggles. However, Giggles wasn’t your typical dragon; he loved cracking jokes more than hoarding gold..."  
```

---

## **2. Key Principles and Tactics** (25 Minutes)

### 🔑 **Principle 1: Clarity in Prompt**

#### **Tactic 1: Use Delimiters 🖋️**

- Always specify the delimiters you are using.
- Example:

```markdown
Prompt:  
"Extract the main idea from the text enclosed by triple curly braces:  
{{{Artificial Intelligence is a branch of computer science focused on creating intelligent systems. These systems can solve problems and make decisions like humans.}}}"  
```

#### **Tactic 2: Ask for Structured Output 📋**

- Provide a clear structure to guide the response.
- Example:

```markdown
Prompt:  
"Introduce a book with the following details:  
- Title  
- Author  
- Genre  
- Brief synopsis  
Provide the output in this structured format:  
- **Title**:  
- **Author**:  
- **Genre**:  
- **Synopsis**:  
"  
```

#### **Tactic 3: Verify Conditions ✔️**

- Check if the input follows a specific pattern and define actions if not.
- Example:

```markdown
Prompt:  
"If the text does not contain a properly formatted date (YYYY-MM-DD), respond with 'Invalid date format.' Otherwise, extract the date."  
```

#### **Tactic 4: "Few-shot" Prompting ✨**

- Provide examples to guide the model.
- Example:

```markdown
Prompt:  
"Complete the following sentences based on the pattern:  
1. The sun is bright. → The moon is dim.  
2. The sky is blue. → The grass is green.  
Complete the sentence:  
3. The ocean is deep. →"  
Output:  
3. The ocean is deep. → The mountains are high.  

```

#### **Tactic 5: Provide Task Context 🎯**

- Specify the audience, tone, and purpose of the task.
- Example:

```markdown
Prompt:  
"Write an article introducing renewable energy for a high school science club newsletter. Use a conversational and engaging tone suitable for teenagers."  
```

### 🧠 **Principle 2: Give the Model Time to Think**

#### **Tactic 1: Specify Steps 🛠️**

- Provide clear steps to guide the model.
- Example:

```markdown
Prompt:  
"Guide me through the process of writing a poem step-by-step.  
- The theme is 'nostalgia for childhood.'  
- Help me choose emotions and symbols to express the theme.  
- Provide an initial draft and a method for revising it."  

```

#### **Tactic 2: Encourage Independent Thinking 🤔**

- Prompt the model to evaluate possibilities before answering.
- Example:

```markdown
Prompt:  
"Think about the advantages and disadvantages of electric cars before answering: 'Should we invest more in electric vehicles?'"  
```

---

## **3. Iterative Prompt Engineering Cycle** (10 Minutes)

### 📜 **Example: Summarization**

Start with:

```markdown
Prompt: "Summarize this article: [Insert article text]."  
```

Improve iteratively:

```markdown
Prompt: "Summarize the following article in under 100 words. Focus on key arguments: [Insert article text]."  
```

---

## **4. Applications: Summarization and Extraction** (10 Minutes)

### 🔄 **Extract vs. Summarize**

- When summarizing, the keyword "extract" can sometimes yield more concise results.

#### **Example**:

```markdown
Prompt:  
"Extract the three main points from this passage: [Insert text]."  
```

---

## **5. Personal Use Case: Empowering Learning with GPT** (5 Minutes)

### 💡 **Examples with Context**

1. **Brainstorming**  
    **Context**: Planning a community coding workshop for teenagers.
    
```markdown
Prompt:  
"Suggest five creative and interactive ways to teach Python basics to high school students at a weekend workshop."  
```
    
2. **Understanding Complex Concepts**  
    **Context**: Learning about challenging topics in physics.
    
```markdown
Prompt:  
"Explain the theory of relativity to a high school student using a relatable analogy and simple terms."  
```
    
3. **Writing Drafts**  
    **Context**: Preparing an essay introduction for a school debate on AI ethics.
    
```markdown
Prompt:  
"Draft an engaging introduction for an essay on how artificial intelligence impacts privacy in modern society. Include a rhetorical question to hook the reader."  
```
    

---

## **6. Responsibility in Using GPT** (5 Minutes)

### 🌟 Key Takeaways:

- Use GPT responsibly.
- Avoid over-reliance; verify outputs for accuracy.
- Balance AI assistance with critical thinking and creativity.

---

## **7. Hands-On Activity** (10 Minutes)

### 🧩 Materials:

A concept

```markdown
"Artificial Intelligence (AI) is a field of computer science focused on building systems capable of performing tasks that typically require human intelligence. Recent advancements have made AI more accessible, impacting industries from healthcare to finance."  
```

product manual

```markdown
"The EcoPro Water Filter is designed to purify drinking water efficiently. Setup is simple: attach the filter to your faucet, twist until secure, and run water through for 30 seconds. Replace the filter every three months. The filter removes 99% of contaminants, including lead and chlorine, ensuring safe drinking water for your family."

```

Historical text

```markdown
"In 1969, humanity took its first steps on the moon during the Apollo 11 mission. Neil Armstrong, the first human to set foot on the lunar surface, declared, 'That’s one small step for man, one giant leap for mankind.' This achievement was the result of years of innovation and international cooperation, marking a milestone in space exploration."
```

go generate some by yourself!

**Exercise Prompt**:

```markdown
"Summarize the above text in two bullet points."  
```

---

## Reference

https://learn.deeplearning.ai/courses/chatgpt-prompt-eng

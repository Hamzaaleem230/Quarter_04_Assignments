# 📘 Assignment 3  
## Mixture-of-Experts (MoE) • Prompt Engineering • Six-Part Prompting • Testing Framework

---

## 1. Reading Material (Before Next Class)

- **Mixture-of-Experts (MoE) and Prompt Engineering**  
- **Six-Part Prompting Framework**  
- **Context Engineering Guide**  
- **AI-Driven & AI-Native Development Presentation**

> Recommended: Review these resources carefully before next class to understand advanced prompting techniques, MoE, and context-aware AI development.

---

## 2. Presentation: Fundamental & Advanced Prompting + MoE

### 2.1 Fundamental Prompting Techniques

1. **Clear & Specific Instructions**  
   Example: “Explain blockchain in simple words suitable for a 10-year-old.”

2. **Role-Based Prompts**  
   Example: “You are a senior JavaScript instructor. Explain closures.”

3. **Step-by-Step Reasoning (Chain-of-Thought)**  
   Break complex tasks into steps for higher accuracy.

4. **Few-Shot Prompting**  
   Provide examples for pattern learning:  
   ```
   Convert: I am happy → I'm happy  
   Convert: I am ready → ?
   ```

5. **Constraints & Formatting**  
   Example: “Summarize this article in 3 bullet points.”

---

### 2.2 Advanced Prompting Strategies

1. **Prompt Chaining** – Divide complex tasks into multiple prompt steps.  
2. **Self-Consistency** – Generate multiple outputs and select the best.  
3. **Retrieval-Augmented Prompting (RAG)** – Combine context + prompt for factual accuracy.  
4. **System + Developer + User Messages** – Structured multi-layer prompting.  
5. **Parameter Tuning** – Temperature, top-p, max tokens affect output behavior.  
6. **Agentic Prompting** – Model performs autonomous tasks with sub-goals and steps.

---

### 2.3 Mixture-of-Experts (MoE)

- MoE = multiple specialized “experts” networks + gating network.  
- Input determines which experts activate.  
- Sparse computation → faster and efficient.  
- Enables trillion-parameter models.

**How MoE Works:**
1. Input arrives  
2. Gating network chooses top experts  
3. Top experts activated  
4. Outputs merged for final response  

**Benefits:**
- Large-scale AI without extreme compute  
- Higher accuracy via specialized experts  
- Scalable for modern LLMs

---

## 3. Videos to Watch

- **How To Use ChatGPT The RIGHT WAY In 2025**  
  Topics: Prompt structuring, memory & context shaping, multi-step reasoning, role prompting.

- **Context Engineering Clearly Explained**  
  Topics: Context window, token prioritization, context packing, retrieval + hybrid prompts.

---

## 4. Testing Framework

**Objective:** Evaluate and document behavior of multiple prompt versions for a task.  

**Chosen Task:** Generate a motivational quote about consistency.

**Instructions:**
- Select base prompt  
- Create multiple versions by adjusting tone, phrasing, model, temperature  
- Test each version systematically  
- Record outputs in a table  
- Add observations

---

### Testing Table

| Prompt Version | Goal | Model | Temperature | Output Quality | Notes |
|----------------|------|--------|-------------|----------------|-------|
| v1.0 | Simple quote | GPT-4 | 0.7 | Good | Generic |
| v1.1 | Emotional tone | GPT-4 | 0.7 | Better | More impact |
| v1.2 | Poetic style | GPT-4 | 0.9 | Creative | Slightly abstract |
| v2.0 | Professional | GPT-5 | 0.5 | Very clear | Polished |
| v2.1 | Modern/youthful | GPT-5 | 0.8 | Engaging | Informal |
| v3.0 | 7-word quote | GPT-5 | 0.4 | Crisp | Minimal |

---

### Prompt Versions

**v1.0:** Write a motivational quote about consistency.  
**v1.1:** Write an emotionally uplifting motivational quote about consistency.  
**v1.2:** Write a poetic, imagery-rich motivational quote about consistency.  
**v2.0:** As a professional author, write a concise motivational quote about consistency.  
**v2.1:** Write a modern, youthful, social-media-style motivational quote about consistency.  
**v3.0:** Write a 7-word motivational quote about consistency.

---

### Observations

- Tone guidance improves output quality  
- Higher temperature → more creative, less controlled  
- GPT-5 outputs more stable and structured than GPT-4  
- Role-based prompts give professional output  
- Short/simple prompts produce generic responses

---
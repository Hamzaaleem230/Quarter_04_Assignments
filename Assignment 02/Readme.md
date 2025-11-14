# 📘 Assignment 2  
## Prompt Engineering • Advanced Strategies • Mixture-of-Experts • Testing Framework

---

## 1. Fundamental Prompting Techniques

### 1. Clear & Specific Instructions  
Achi output tab milti hai jab task bilkul clearly define ho.  
**Example:**  
Explain blockchain in simple words suitable for a 10-year-old.

---

### 2. Role-Based Prompts  
Model ko role dene se tone aur expertise improve hoti hai.  
**Example:**  
You are a senior JavaScript instructor. Explain closures.

---

### 3. Step-by-Step Reasoning (Chain-of-Thought)  
Complex tasks ko steps me tod kar explain karwana accuracy barhata hai.

---

### 4. Few-Shot Prompting  
Examples de kar model ko pattern sikhaya jata hai.

**Example:**
```
Convert: I am happy → I'm happy  
Convert: I am ready → ?
```

---

### 5. Constraints & Formatting  
Model ko exact output format batao → best, clean result.

**Example:**  
Summarize this article in 3 bullet points.

---

---

## 2. Advanced Prompting Strategies

### 1. Prompt Chaining  
Ek complex task ko multiple prompts me divide karna.

### 2. Self-Consistency  
Multiple outputs generate karke best pick karna.

### 3. Retrieval-Augmented Prompting (RAG)  
Context + prompt → factual accuracy improve.

### 4. System + Developer + User Messages  
Output ko structured aur controlled banata hai.

### 5. Parameter Tuning  
Temperature, top-p, max tokens → behavior change hota hai.

### 6. Agentic Prompting  
Model ko goals, steps, and tools de kar tasks autonomously solve karwana.

---

---

## 3. Mixture-of-Experts (MoE)

MoE aik neural architecture hai jisme multiple “experts” hotay hain.  
Input ke mutabiq **gating network** decide karta hai kaunse experts activate honge.

### How MoE Works
1. Input aata hai  
2. Gating network relevant experts choose karta hai  
3. Sirf top experts activate hote hain (sparse computing)  
4. Output merge hota hai  

### Why MoE is Important
- Huge models without extreme compute  
- Faster inference  
- Specialized experts → better accuracy  
- Enables trillion-parameter LLMs

---

---

## 4. Video Summaries

### **How To Use ChatGPT the Right Way (2025)**  
- Prompt structure importance  
- Multi-step reasoning  
- Role prompting  
- Context handling  
- Practical examples

### **Context Engineering Clearly Explained**  
- Context window kya hoti hai  
- Token prioritization  
- Context packing & compression  
- RAG + prompting hybrid approach

---

---

## 5. Testing Framework  
**Task Chosen:** Generate a motivational quote about consistency.

---

## Testing Table

| Prompt Version | Goal | Model | Temp | Output Quality | Notes |
|----------------|------|--------|-------|----------------|--------|
| v1.0 | Simple quote | GPT-4 | 0.7 | Good | Generic |
| v1.1 | Emotional tone | GPT-4 | 0.7 | Better | More impact |
| v1.2 | Poetic style | GPT-4 | 0.9 | Creative | Slightly abstract |
| v2.0 | Professional | GPT-5 | 0.5 | Very clear | Polished |
| v2.1 | Modern/youthful | GPT-5 | 0.8 | Engaging | Informal |
| v3.0 | 7-word quote | GPT-5 | 0.4 | Crisp | Minimal |

---

## Prompt Versions

### v1.0  
Write a motivational quote about consistency.

### v1.1  
Write an emotionally uplifting motivational quote about consistency.

### v1.2  
Write a poetic, imagery-rich motivational quote about consistency.

### v2.0  
As a professional author, write a concise motivational quote about consistency.

### v2.1  
Write a modern, youthful, social-media-style motivational quote about consistency.

### v3.0  
Write a 7-word motivational quote about consistency.

---

## Observations

- Tone guidance se output quality improve ho jati hai.  
- Higher temperature → creative but less controlled output.  
- GPT-5 ka structure aur grammar more stable tha.  
- Role prompting se professional quality output aata hai.  
- Short prompts zyada generic results dete hain.

---
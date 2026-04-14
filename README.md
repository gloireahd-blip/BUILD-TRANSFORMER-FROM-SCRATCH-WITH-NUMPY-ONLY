# BUILD TRANSFORMER FROM SCRATCH 

# 🧠 Transformer from Scratch: The Engine Behind GPT, Gemini & DeepSeek (LLM)

<center>

## 🚀 Project Overview
Have you ever wondered what actually happens inside the "brain" of **ChatGPT**, **Gemini**, or **DeepSeek**? 
Curieux de découvrir la mécanique interne qui anime des modèles comme ChatGPT, Gemini ou DeepSeek ?

This project is a deep-dive implementation of the **Transformer architecture**, built entirely **from scratch using only NumPy**. No high-level libraries like PyTorch or TensorFlow—just pure Linear Algebra, Calculus, and Python.

### 🔬 Why "From Scratch"?
To master AI, you must understand the "mechanical assembly" of its neurons. By implementing the core math, I’ve demystified how Large Language Models (LLMs) process language, manage context, and "understand" relationships between words.

---

## 🛠 The Mathematical Blueprint

### 1. Scaled Dot-Product Attention
The "Secret Sauce" of LLMs. It allows the model to dynamically focus on different words in a sentence.

$$Attention(Q, K, V) = \text{softmax}\left(\frac{Q \cdot K^T}{\sqrt{d_{model}}}\right)V$$

### 2. The Learning Objective (Cross-Entropy)
How the model measures its own mistakes during training:

$$L = -\sum_{k=0}^{n} Y_k \cdot \ln(P_k)$$

### 3. Gradient Descent Optimization
The process of "tuning the engine" to minimize error:

$$W_{i+1} = W_i - \eta \cdot \frac{\partial L}{\partial W_i}$$

</center>

---

## 📊 Experimental Results: "Je pars à Paris"

I trained this model for **450 epochs** on a sample sequence. The results perfectly illustrate the power of the Attention mechanism:



* **The "Yellow Square" Effect:** As seen in the visualizations, the model creates high-intensity connections (scores > 0.8) represented by **yellow squares**.
* **Semantic Mapping:** In the phrase *"Je pars à Paris"*, the model successfully linked the subject (**Je**) to the verb (**pars**). This "bridge" is exactly how GPT knows who is performing an action in a complex story.
* **Contextual Intelligence:** The model isn't just memorizing words; it's learning the **logical structure** of the language through matrix multiplications.

## 💡 Conclusion
Building this "brain" from scratch confirms that Transformers are not black boxes—they are elegant mathematical machines. This project serves as a foundation for my journey into becoming a Machine Learning Engineer.

---
**Tech Stack:** Python, NumPy, Matplotlib (for visualization).


<img width="864" height="438" alt="is al youneed corurbe" src="https://github.com/user-attachments/assets/9f55e04b-7821-4649-bd1e-39eea363129f" />
<img width="858" height="383" alt="w_k" src="https://github.com/user-attachments/assets/22c5048c-0156-486d-994d-3279640279f3" />



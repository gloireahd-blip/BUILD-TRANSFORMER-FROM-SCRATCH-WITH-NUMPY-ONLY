# BUILD TRANSFORMER FROM SCRATCH 

## Transformer Mechanics: Building from Scratch with NumPy

<center>

## Core Mathematical Foundations

### 1. Scaled Dot-Product Attention
The heart of the model is the attention mechanism, which allows tokens to interact and focus on relevant parts of the sequence.

$$Attention(Q, K, V) = \text{softmax}\left(\frac{Q \cdot K^T}{\sqrt{d_{model}}}\right)V$$

### 2. Loss Function (Cross-Entropy)
To measure the gap between predictions and reality, we use the Cross-Entropy loss:

$$L = -\sum_{k=0}^{n} Y_k \cdot \ln(P_k)$$

### 3. Optimization (Gradient Descent)
The weights are updated by moving in the opposite direction of the gradient:

$$W_{i+1} = W_i - \eta \cdot \frac{\partial L}{\partial W_i}$$

</center>

---

## Experimental Results: Sentence Analysis

For this implementation, I tested the model with the French sentence: **"Je pars à Paris"**.

### Key Observations from the Attention Matrix ($A$):
After training for only **450 epochs**, the model reached a stable state. As shown in the generated figures, the **yellow squares** represent the strongest connections, where the attention score is at its maximum (above **0.8**).

* **Strong Semantic Link:** A prominent yellow square is visible at the intersection of **"Je"** (Subject) and **"pars"** (Verb). As the figures show, this high-intensity connection proves that the model learned the relationship between the subject and the action.
* **Contextual Understanding:** This demonstrates that to "understand" the sentence, the model focuses heavily on the link between "Je" and "pars" rather than just treating words as isolated units.
* **Entity Anchoring:** We also observe yellow squares for **"Paris"**, which acts as a stable anchor for the sentence's destination meaning.

### Conclusion
By building this Transformer using only **NumPy**, I demonstrated that the attention mechanism is not a black box. The heatmaps clearly visualize how the model learns grammar and logic through matrix multiplications, effectively "seeing" which words must be linked together to capture the full context.


<img width="864" height="438" alt="is al youneed corurbe" src="https://github.com/user-attachments/assets/9f55e04b-7821-4649-bd1e-39eea363129f" />
<img width="858" height="383" alt="w_k" src="https://github.com/user-attachments/assets/22c5048c-0156-486d-994d-3279640279f3" />



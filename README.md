# CortexDesk 

**CortexDesk** is a lightweight intent-based conversational AI built with Python and Keras, designed to demonstrate how classical NLP pipelines can power responsive desktop chat assistants without relying on large language models.

It focuses on one important engineering idea:

> You don’t always need massive models to build useful AI systems — sometimes a well-designed pipeline is enough.

---

##  Overview

CortexDesk is an end‑to‑end chatbot system that:

* Processes natural language using tokenization + lemmatization
* Converts text into Bag‑of‑Words vectors
* Classifies user intent via a neural network
* Selects contextual responses dynamically
* Runs inside a desktop GUI using Tkinter

This project is ideal for understanding the **foundations of conversational AI systems** before jumping into transformer-heavy stacks.

---

##  Architecture

**Pipeline:**

User Input → Text Preprocessing → Feature Vector (BoW) → Neural Network → Intent Prediction → Response Selection → UI Output

### Model

* Feedforward Neural Network
* Dense layers with Dropout for regularization
* Softmax output for multi-class intent prediction
* SGD optimizer with momentum

Designed to balance:

✅ Simplicity
✅ Interpretability
✅ Fast training
✅ Low compute requirements

---

##  Tech Stack

* Python
* NLTK
* NumPy
* Keras / TensorFlow
* Tkinter

---

##  Key Features

✔ Intent classification from scratch
✔ Custom training pipeline
✔ Persistent vocabulary + class artifacts
✔ Confidence thresholding
✔ Rule-based fallback matching
✔ Desktop chat interface

---

##  Why This Project Matters

Most beginners jump directly into LLM APIs.

But production engineers know:

👉 Understanding classical NLP builds stronger intuition.
👉 Not every product needs a transformer.
👉 Latency, cost, and control still matter.

CortexDesk demonstrates how much you can build **before** reaching for large models.

---

##  Installation

```bash
git clone https://github.com/yourusername/cortexdesk.git
cd cortexdesk
pip install -r requirements.txt
```

Download required NLTK resources:

```python
import nltk
nltk.download('punkt')
nltk.download('wordnet')
```

---

##  Usage

### Train the model

```bash
python train.py
```

### Launch the chatbot

```bash
python app.py
```

---

##  Who Is This For?

* AI / ML students
* NLP beginners
* Engineers exploring chatbot mechanics
* Developers who want to understand intent systems
* Anyone building AI without GPU-heavy infrastructure

---

##  Future Improvements

* Replace BoW with embeddings
* Add transformer-based intent comparison
* Memory + conversation state
* REST API deployment
* Dockerization
* Vector search integration

---

##  Contributing

Contributions, experiments, and architectural improvements are welcome.

If you build something on top of CortexDesk — I’d love to see it.

---

##  Final Thought

Great AI engineers aren’t defined by the size of their models…

…but by their ability to design systems.


# 🤖 Agentic AI Hiring Assistant for Startups (No Offer Letter)

This project delivers a fully functioning **agentic AI application** that helps HR professionals design and manage a hiring plan for startups using **LangGraph**, **LangChain**, and **OpenAI Function Calling**. It features intelligent multi-step reasoning, simulated tool use, analytics, memory, and a user-friendly Gradio interface.

---

## ✅ Features

| Category | What you get |
|----------|--------------|
| **Multi-step reasoning** | LangGraph workflow: JD → Funnel → Drop-off → Salary |
| **Tool simulation** | Funnel analytics + salary estimator |
| **Memory retention** | State passed between nodes via `TypedDict` |
| **Frontend** | Gradio Blocks UI with custom theme |
| **Analytics** | Matplotlib bar chart for candidate drop-off |

---

## 📦 Architecture

1. **LangGraph** – orchestrates the step-by-step hiring plan.  
2. **LangChain + OpenAI** – GPT-4o powers content generation.  
3. **Gradio** – launches an in-notebook web app.  
4. **Matplotlib** – renders the analytics chart.

```
(Job Role) ─▶ [Generate JD] ─▶ [Funnel] ─▶ [Drop-off %] ─▶ [Salary Range]
```

---

## 🚀 Getting Started

1. **Install packages**

```bash
pip install langgraph langchain openai gradio matplotlib
```

2. **Set your OpenAI key**

```python
import os
os.environ["OPENAI_API_KEY"] = "sk-..."   # your key here
```

3. **Run the notebook**

Open `agentic_hr_app.ipynb` in Google Colab or Jupyter and run all cells.  
A Gradio link will appear; open it to use the app.

---

## 📊 What the App Produces

- **📄 Job Description** – full, ready-to-publish JD  
- **💼 Salary Estimate** – competitive range for the role  
- **📉 Drop-off Chart** – visual candidate attrition per stage  

---

## 🌟 Bonus Extensions

- Swap the static funnel with real ATS data (Greenhouse, Lever).  
- Persist conversations in a vector store for long-term memory.  
- Deploy the Gradio app on Hugging Face Spaces or Render.

---

## 🧠 Why It’s Agentic

- **Reasoning graph**: each node acts autonomously yet in sequence.  
- **Tool integration**: simulated analytics functions behave like external tools.  
- **Memory**: state object passes knowledge between steps, enabling context-aware decisions.

---

Made with ❤️ using LangGraph, LangChain, Gradio, and OpenAI.

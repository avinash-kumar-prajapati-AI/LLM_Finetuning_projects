# 🧠 LLM-Driven Windows UI Automation Agent  
### Natural Language → Executable UI Actions (Local, Safe, Deterministic)

> **An end-to-end project that fine-tunes a Large Language Model to convert natural language instructions into structured Windows UI automation steps, executed safely via `pywin32`.**

⭐ Built for **applied LLM engineering**, **agent systems**, and **real-world automation**  
⭐ Fully **local**, **offline**, and **deterministic**  
⭐ Focused on **structure, safety, and execution**, not chat demos

---

## 🚀 Why This Project Matters

Most LLM demos stop at *text generation*.  
This project goes further:

✅ Turns **natural language → machine-executable plans**  
✅ Uses **instruction fine-tuning + LoRA**, not prompting tricks  
✅ Produces **strict JSON contracts**, not free text  
✅ Separates **planning (LLM)** from **execution (OS APIs)**  
✅ Runs **locally** (no cloud, no API keys)

This is how **real agent systems** are built.

---

## 🎯 What This Solves

Traditional UI automation requires:
- brittle scripts
- hard-coded flows
- manual maintenance per app

This system enables:

> **“Open Notepad and close it”**  
⬇️  
```json
{
  "application": "notepad",
  "actions": [
    {"action": "open_app", "app": "notepad"},
    {"action": "hotkey", "keys": "alt+f4"}
  ]
}
```

#### 🧠 Key Engineering Concepts Demonstrated

- Instruction fine-tuning (not chat fine-tuning)

- LoRA / PEFT for efficient training

- Quantized LLMs (4-bit)

- Deterministic decoding

- Output constraint & validation

- JSON-only model contracts

- Agent design: Planner vs Executor

- Windows automation using pywin32
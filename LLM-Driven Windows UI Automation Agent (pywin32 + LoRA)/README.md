# 🧠 LLM-Driven Windows UI Automation Agent  
### Natural Language → Executable UI Actions (Local, Safe, Deterministic)

> **An end-to-end applied LLM project that fine-tunes a Large Language Model to convert natural language instructions into structured Windows UI automation steps, executed safely using `pywin32`.**

⭐ Built for **applied LLM engineering**, **agent systems**, and **real-world automation**  
⭐ Fully **local**, **offline**, and **deterministic**  
⭐ Focused on **structure, safety, and execution** — not chat demos

---

## 🚀 Why This Project Matters

Most LLM projects stop at text generation.

This project goes further by building a **real AI agent pipeline**:

- Converts **natural language → executable action plans**
- Uses **instruction fine-tuning + LoRA**, not prompt tricks
- Produces **strict JSON outputs**, not free-form text
- Separates **planning (LLM)** from **execution (OS APIs)**
- Runs **locally** (no cloud APIs, no vendor lock-in)

---

## 🎯 What Problem Does This Solve?

Traditional UI automation requires:
- brittle scripts
- manual hardcoding per app
- frequent maintenance

This system enables:

**User command**
```
Open Notepad and close it
```

**Model output**
```json
{
  "application": "notepad",
  "actions": [
    {"action": "open_app", "app": "notepad"},
    {"action": "hotkey", "keys": "alt+f4"}
  ]
}
```

---

## 🏗️ System Architecture

User Instruction → Fine-Tuned LLM (LoRA) → JSON Plan → Validator → pywin32 Executor(future scope by mapping generated model output to pywin32 funtion features) → Real UI Automation

---

## ⚙️ Tech Stack

- torch, transformers, datasets
- peft, trl, unsloth
- pandas, openpyxl
- pywin32

---

## ⭐ Final Takeaway

**LLMs are most powerful when used as planners, not executors.**

- This project shows how to build a safe, deterministic, local AI agent.

- How to fine-tune LLMs for structured outputs

- Why decoding control > prompt engineering

- How LoRA enables serious projects on limited hardware

- How to design safe, executable AI agents

- How to bridge LLMs with operating systems responsibly

**Future Improvements**

1. OCR / vision-based UI detection

2. Safer execution sandbox

3. Expanded application coverage

**Who This Project Is For**

- AI / ML Engineers

- Systems & Automation Engineers

- Researchers exploring agent architectures

- Students building real LLM systems

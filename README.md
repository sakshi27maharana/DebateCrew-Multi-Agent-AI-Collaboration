---

# 🧠 DebateCrew: Multi-Agent AI Collaboration

Welcome to **DebateCrew** — a powerful template built on [crewAI](https://crewai.com) that makes setting up **multi-agent AI systems** simple, flexible, and impactful.

With DebateCrew, you can orchestrate intelligent agents that collaborate on complex tasks — combining their strengths to maximize collective intelligence.

---

## 🛠️ Installation

### Requirements

* **Python**: `>=3.10` and `<3.14`
* **Dependency Manager**: [UV](https://docs.astral.sh/uv/)

### Step 1: Install UV

If not already installed, run:

```bash
pip install uv
```

### Step 2: Install Dependencies

Navigate to your project folder and install requirements:

```bash
uv pip install -r requirements.txt
```

Or, lock dependencies and install via the CLI:

```bash
crewai install
```

---

## ⚙️ Customization

Before running the crew, configure it to match your needs:

1. **Set up your API key**

   * Add your `OPENAI_API_KEY` to the `.env` file

2. **Configure your crew**

   * `src/debate/config/agents.yaml` → Define agents
   * `src/debate/config/tasks.yaml` → Define tasks
   * `src/debate/crew.py` → Add logic, tools, and custom arguments
   * `src/debate/main.py` → Customize agent/task inputs

---

## ▶️ Running DebateCrew

From the project root, run:

```bash
crewai run
```

This command will:

* Initialize your crew of agents
* Assign them tasks as defined in your configs
* Generate a `report.md` file (default example: research on LLMs)

---

## 🤝 Understanding Your Crew

A **crew** is a group of specialized AI agents:

* Each agent has **roles, goals, and tools**
* Tasks are orchestrated through `config/tasks.yaml`
* Capabilities and configurations live in `config/agents.yaml`

The crew collaborates intelligently to achieve complex objectives.

---

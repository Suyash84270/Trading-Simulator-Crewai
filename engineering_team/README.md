# EngineeringTeam Crew – Trading Simulation Platform

Welcome to the **EngineeringTeam Crew** project, powered by [crewAI](https://crewai.com). This project demonstrates a multi-agent AI system orchestrating the development of a **Trading Simulation Account Management Platform**, showcasing a full development pipeline from **requirements → design → backend implementation → frontend demo → testing**, all automated via AI agents.

You can try the live demo on **Hugging Face Spaces**: [suyashsharma/trading-simulator](https://huggingface.co/spaces/suyashsharma/trading-simulator)

---

## Project Overview

This project simulates a **trading account management system** where users can:

- Create an account with an initial deposit
- Deposit or withdraw funds
- Buy or sell shares (AAPL, TSLA, GOOGL)
- Track portfolio value, profit/loss, holdings, and transaction history

The project demonstrates **multi-agent AI collaboration**:

1. **Engineering Lead Agent** – Converts requirements into a detailed backend design  
2. **Backend Engineer Agent** – Implements the backend as a Python module  
3. **Frontend Engineer Agent** – Creates a Gradio UI for interactive demonstration  
4. **Test Engineer Agent** – Generates unit tests for backend verification  

The agents execute tasks **sequentially**, simulating a collaborative development workflow.

---

## Project Flow

**Step 1 – Requirements & Design:**  
The Engineering Lead reads high-level requirements and outputs a detailed Python module design (`accounts.py_designed.md`) with classes, functions, and method signatures.

**Step 2 – Backend Implementation:**  
The Backend Engineer takes the design and creates `accounts.py`, implementing all features like account management, deposits, withdrawals, buy/sell shares, portfolio calculations, and transaction history.

**Step 3 – Frontend Demo:**  
The Frontend Engineer creates a **Gradio UI (`app.py`)** for interaction with the backend, including:

- Account creation
- Deposit/withdraw funds
- Buy/sell shares
- Portfolio summary, profit/loss, holdings, transactions

**Step 4 – Testing:**  
The Test Engineer generates `test_accounts.py` with unit tests to ensure all backend functionality works correctly.

---

## Project Structure

engineering_team/
├── config/
│ ├── agents.yaml # Agent roles, goals, backstories
│ └── tasks.yaml # Task definitions
├── output/
│ ├── accounts.py # Backend module
│ ├── app.py # Gradio frontend
│ ├── test_accounts.py # Unit tests
│ └── *_design.md # Backend design from Engineering Lead
├── crew.py # Defines agents and task orchestration
├── main.py # Runs the multi-agent workflow
└── README.md


---

## Techniques & Tools Used

- **AI Agents (crewAI)** – Auto-generates design, backend, UI, tests  
- **Python 3.10–3.13**  
- **Gradio** – Interactive UI layer  
- **Unit Testing** for backend validation  
- **Sequential Multi-Agent Workflow**  

---

## Installation

### **Prerequisites:**  
Python 3.10–3.13

### Install `uv` dependency manager:

\`\`\`bash
pip install uv
\`\`\`

---

## Running the Project

### **Run the full multi-agent workflow**  
This will execute design → backend → frontend → testing:

\`\`\`bash
python main.py
\`\`\`

This generates:

- `accounts.py_designed.md`  
- `accounts.py`  
- `app.py`  
- `test_accounts.py`  

---

### **Launch the Gradio Frontend**

\`\`\`bash
python output/app.py
\`\`\`

---

## Features

### **Backend (`accounts.py`)**
- Account creation with initial deposit  
- Deposit & withdrawal handling  
- Buy/sell shares (AAPL, TSLA, GOOGL)  
- Portfolio value & profit/loss calculation  
- Transaction history logging  

### **Frontend (`app.py`)**
- Built using Gradio  
- Clean, simple UI  
- Allows: create account, deposit, withdraw, buy, sell  
- Displays: holdings, profit/loss, portfolio value  

---

## AI Agent Roles

| Agent             | Role                    | Task          |
|------------------|--------------------------|---------------|
| Engineering Lead  | Design backend           | design_task   |
| Backend Engineer  | Implement Python module  | code_task     |
| Frontend Engineer | Build Gradio UI          | frontend_task |
| Test Engineer     | Write unit tests         | test_task     |

---

## Screenshots / Demo

> Replace with your actual images:

![App Screenshot](assets/screenshot.png)



---

## Hugging Face Space

Run the live demo instantly:  
**https://huggingface.co/spaces/suyashsharma/trading-simulator**

---

## Customization

- Modify `agents.yaml` → edit agent roles & prompts  
- Modify `tasks.yaml` → change tasks  
- Update `crew.py` → update orchestration  
- Extend `accounts.py` → add advanced trading logic  

---

## Learning Outcomes

- Build a **multi-agent AI-driven development pipeline**  
- Understand the full cycle: design → backend → UI → testing  
- Learn Gradio-based UI development  
- Learn agent collaboration strategies  

---

## License

This project is open-source and free to use for learning and demonstration purposes.

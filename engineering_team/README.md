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

- **AI Agents (crewAI)** – Automates design, coding, frontend, and testing  
- **Python 3.10–3.13** – Backend implementation  
- **Gradio** – Interactive frontend for demonstration  
- **Unit Testing** – Ensures backend reliability  
- **Multi-Agent Workflow** – Sequential agent execution simulating a software team  

---

## Installation

**Prerequisites:** Python 3.10–3.13  

1. Install `uv` for dependency management:

```bash
pip install uv






## Running the Project

 ### Run the full multi-agent workflow:

 --This will generate:

-accounts.py_designed.md → Backend design

-accounts.py → Python module for trading account management

-app.py → Gradio frontend

-test_accounts.py → Unit tests






## Features

### Backend (accounts.py)

-Account creation with initial deposit

-Deposit and withdrawal handling

-Buy/sell shares (AAPL, TSLA, GOOGL)

-Track portfolio value and profit/loss

-List transaction history

### Frontend (app.py)

-Built with Gradio for a simple, interactive UI

-Demo user actions: deposit, withdraw, buy/sell shares

-View portfolio, holdings, P/L, and transactions






# AI Agent Roles

| Agent             | Role                    | Task          |
| ----------------- | ----------------------- | ------------- |
| Engineering Lead  | Design backend          | design_task   |
| Backend Engineer  | Implement Python module | code_task     |
| Frontend Engineer | Build Gradio UI         | frontend_task |
| Test Engineer     | Write unit tests        | test_task     |




## Screenshots / Demo

![App Screenshot](assets/images/screenshot.png):<img width="1217" height="815" alt="Screenshot 2025-11-13 134117" src="https://github.com/user-attachments/assets/924ef9fa-15a4-44b2-9009-8fe03e0ac933" />





## Hugging Face Space

### Run the live demo without setup:
[Trading Simulator Demo](https://huggingface.co/spaces/suyashsharma/trading-simulator)



## Customization

-Update agents.yaml to change agent roles or goals

-Update tasks.yaml to adjust tasks

-Modify crew.py to customize agent orchestration

-Extend accounts.py to add more trading features


##Learning Outcomes

-Build a multi-agent AI workflow to implement a full application

-Experience the design → implementation → frontend → testing cycle

-Learn Gradio for interactive frontend demos

-Understand AI collaboration for software development





## License

This project is open-source and free to use for learning and demonstration purposes.

# AI Hiring Assistant System

An AI-powered Hiring Assistant built using **LangGraph** and **OpenAI** that automates the hiring process by analyzing resumes, matching candidates with job requirements, performing HR review, generating interview questions, and providing a final hiring recommendation.

---

## Features

- Resume Analysis
- Job Description Matching
- Candidate Skill Evaluation
- Human-in-the-Loop HR Review
- Interview Question Generation
- Final Hiring Recommendation
- LangGraph Workflow Orchestration

---

## Workflow

```
Resume Analysis
        │
        ▼
Skill Match Evaluation
        │
        ▼
HR Review (Human Approval)
        │
        ▼
Interview Question Generation
        │
        ▼
Final Hiring Decision
```

---

## Technologies Used

- Python
- LangGraph
- LangChain
- OpenAI
- Pydantic
- Jupyter Notebook

---

## Prerequisites

- Python 3.11 or later
- Git
- Jupyter Notebook
- OpenAI-compatible API Key
- OpenAI-compatible Base URL

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/AI-Hiring-Assistant.git
cd AI-Hiring-Assistant
```

---

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3. Configure Environment Variables

Create a file named **`.env`** in the project root.

Example:

```env
OPENAI_API_KEY=your_api_key_here
OPENAI_BASE_URL=https://api.openai.com/v1
```

Replace the values with your own credentials.

**Example**

```env
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
OPENAI_BASE_URL=https://api.openai.com/v1
```

> **Note:** If you are using another OpenAI-compatible provider, replace the Base URL accordingly.

---

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook:

```
Hiring Agent.ipynb
```

---

### 5. Run the Notebook

Run all cells from top to bottom.

The workflow will:

- Analyze the candidate's resume
- Compare it with the job description
- Evaluate candidate skills
- Perform HR review
- Generate interview questions
- Produce the final hiring recommendation

---

## Project Structure

```
AI-Hiring-Assistant/
│
├── Hiring Agent.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── .env (Create this file yourself)
```

---

## Environment Variables

| Variable | Description |
|----------|-------------|
| `OPENAI_API_KEY` | Your OpenAI-compatible API Key |
| `OPENAI_BASE_URL` | API Base URL |

---

## requirements.txt

```text
langgraph
langchain
langchain-openai
openai
python-dotenv
pydantic
jupyter
ipykernel
```

---

## Notes

- This repository does **not** include API keys.
- Create your own `.env` file before running the project.
- Never commit your `.env` file to GitHub.
- This project is intended for learning LangGraph workflows, state management, and human-in-the-loop AI applications.

---

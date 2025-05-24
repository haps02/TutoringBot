# 🧠 TutoringBot – Multi-Agent AI Tutoring System

This is a full-stack multi-agent AI tutoring system built with a React frontend (`TutoringBot-fe`) and a Python backend (`TutoringBot-be`). The system intelligently delegates user queries to specialized tutoring agents via a Root Agent, making learning interactive and personalized.

---

## ⚙️ Architecture Overview

The system is built using Google's **Gemini API** and the **ADK (Agent Development Kit)** framework to support modular, multi-agent behavior.

### 🧩 Agents

- **Root Agent**: Receives all user queries and routes them to the appropriate tutor agent.
- **Greeting Agent**: Handles greetings and onboarding.
- **Farewell Agent**: Handles conversation endings and polite exits.
- **Math Tutor Agent**: Handles mathematics-related queries.
- **Physics Tutor Agent**: Handles physics-related queries.
- **Biology Tutor Agent**: Handles biology-related queries.

### 🛠 Tools Used

- **Calculator Tool**: Performs dynamic mathematical calculations.
- **Lookup Table Tool**: Retrieves subject-specific facts or concepts.
- **Load Memory Tool**: Adds contextual memory across interactions.

---

## 🚀 Running the Project Locally

### 🖥 Frontend (`TutoringBot-fe`)

1. Navigate to the frontend directory:
   ```bash
   cd TutoringBot-fe
   
2. Install dependencies:
   ```bash
   npm install
   
3. Start the develpment server
   ```bash
   npm start


### 🧠 Backend (TutoringBot-be)

1. Navigate to the backend directory:

   ```bash
   cd TutoringBot-be
   
2. Create a .env file with the following content:

   GOOGLE_GENAI_USE_VERTEXAI="False"
   GOOGLE_API_KEY="<YOUR_GEMINI_API_KEY>"
   
3. Create and activate a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate

4. Install dependencies:

   ```bash
   pip install -r requirements.txt

5. Start the backend server:

   ```bash
   python api.py

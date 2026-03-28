# 🌿 SafeSpace: AI-Powered Psychological Helper

SafeSpace is an empathetic, AI-driven conversational agent designed to provide a secure and judgment-free environment for users to explore their thoughts, vent, and practice mindfulness. By leveraging advanced Large Language Models (LLMs), it simulates active listening and offers supportive, context-aware responses.

> **⚠️ Medical Disclaimer:** *This application is an experimental artificial intelligence project. It is **not** a substitute for professional medical advice, diagnosis, or therapy. If you are experiencing a mental health crisis, please contact a certified healthcare provider or a local emergency hotline immediately.*

---

## ✨ Features
* **Empathetic Conversational UI:** A clean, calming, and intuitive frontend designed to make users feel at ease.
* **Context-Aware Memory:** The AI retains conversation history during the session to provide relevant, thoughtful follow-ups and active listening.
* **Decoupled Architecture:** Separation of frontend and backend logic for better scalability and maintenance.
* **Ultra-Fast Dependency Management:** Powered by `uv` for lightning-fast, deterministic, and reproducible builds.

---

## 🛠️ Tech Stack
* **Language:** Python 3.10+
* **Package Manager:** [uv](https://github.com/astral-sh/uv)
* **Frontend:** Streamlit / Gradio *(via `frontend.py`)*
* **Backend Core:** FastAPI / LangChain *(via `main.py`)*
* **AI/LLM:** Google Gemini / OpenAI / Anthropic *(Configurable via API)*

---

## 📂 Project Structure

```text
SafeSpace/
├── AI Therapist.pdf     # Project documentation, architecture, and design notes
├── frontend.py          # User interface and client-side conversational logic
├── main.py              # Backend server, API endpoints, and LLM orchestration
├── pyproject.toml       # Project metadata and dependency declarations
├── uv.lock              # Lockfile ensuring deterministic dependency resolution
└── README.md            # Project documentation
```

---

## ⚙️ Getting Started

Follow these instructions to set up and run the project locally. This project uses `uv`, an extremely fast Python package installer and resolver.

### 1. Prerequisites
* Install Python 3.10+.
* Install `uv` on your machine:
  * **Windows:** `powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"`
  * **macOS/Linux:** `curl -LsSf https://astral.sh/uv/install.sh | sh`

### 2. Clone the Repository

```bash
git clone [https://github.com/Sv2972/SafeSpace.git](https://github.com/Sv2972/SafeSpace.git)
cd SafeSpace
```

### 3. Install Dependencies
Using `uv sync` will automatically read the `uv.lock` file, create a virtual environment (`.venv`), and install the exact dependency versions required.

```bash
uv sync
```

### 4. Configure Environment Variables
Create a `.env` file in the root directory and add your required LLM API keys:

```env
# Example using Google Gemini
GEMINI_API_KEY=your_api_key_here

# Example using OpenAI
OPENAI_API_KEY=your_api_key_here
```

---

## 🏃‍♂️ Running the Application

To run the application, you need to activate the virtual environment and start the services.

### 1. Activate the Virtual Environment:

* **Windows:** `.venv\Scripts\activate`
* **macOS/Linux:** `source .venv/bin/activate`

### 2. Start the Backend / Core Logic:
*(Run this in your first terminal)*

```bash
python main.py
```

### 3. Start the Frontend UI:
*(Open a second terminal, activate the virtual environment again, and run your UI framework)*

```bash
# If using Streamlit:
streamlit run frontend.py

# If using Gradio or standard Python:
python frontend.py
```

---

## 🤝 Contributing

Contributions are always welcome! If you have ideas to improve the prompt engineering, add UI features, or optimize the backend pipeline, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📄 License
This project is open-source and available under the MIT License.

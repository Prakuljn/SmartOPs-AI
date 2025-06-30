# 🤖 SmartOps AI – Real-Time Strategy Assistant

SmartOps AI is an intelligent, real-time business strategy assistant that leverages the power of search, summarization, and large language models to deliver actionable strategies for your business goals. With a simple Streamlit web interface, SmartOps AI orchestrates multiple APIs to provide you with the most relevant and insightful recommendations in seconds.

---

## 🚀 Features

- **Google Search Integration:** Fetches the latest and most relevant information using the Serper API.
- **Automated Summarization:** Condenses search results into concise insights via the Tavily API.
- **AI-Powered Strategy Generation:** Utilizes Gemini LLM to craft tailored business strategies.
- **Modern Web UI:** Built with Streamlit for a fast, interactive experience.
- **Modular & Extensible:** Clean codebase with separate modules for each API and workflow.

---

## 🗂️ Project Structure

```
.
├── main.py                # Streamlit app entry point
├── langgraph_flow.py      # Orchestrates the API workflow
├── serper_module.py       # Handles Google search via Serper API
├── tavily_module.py       # Handles summarization via Tavily API
├── gemini_module.py       # Handles LLM responses via Gemini API
├── requirements.txt       # Python dependencies
├── Dockerfile             # Containerization setup
├── .env                   # API keys (not committed)
└── README.md              # Project documentation
```

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/smartops-ai.git
cd smartops-ai
```

### 2. Set Up Environment Variables

Create a `.env` file in the project root with your API keys:
```
SERPER_API_KEY=your_serper_api_key
TAVILY_API_KEY=your_tavily_api_key
GEMINI_API_KEY=your_gemini_api_key
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the App Locally

```bash
streamlit run main.py
```

---

## 🐳 Run with Docker

1. **Build the Docker image:**
   ```bash
   docker build -t smartops-ai .
   ```

2. **Run the container:**
   ```bash
   docker run -p 8501:8501 --env-file .env smartops-ai
   ```

3. **Open your browser and visit:**  
   [http://localhost:8501](http://localhost:8501)

---

## 📦 Dependencies

- Python 3.12
- Streamlit
- LangGraph
- Requests
- python-dotenv

---

## 💡 How It Works

1. **User Input:** Enter your business goal or question.
2. **Search:** The app fetches top search results using Serper.
3. **Summarize:** Tavily API condenses the findings.
4. **Strategize:** Gemini LLM generates a tailored strategy.
5. **Result:** Your smart strategy is displayed instantly.

---

## 🙏 Acknowledgements

- [Streamlit](https://streamlit.io/)
- [Serper API](https://serper.dev/)
- [Tavily API](https://tavily.com/)
- [Gemini LLM](https://ai.google.dev/)

---

> **Empower your business with real-time, AI-driven strategies!**
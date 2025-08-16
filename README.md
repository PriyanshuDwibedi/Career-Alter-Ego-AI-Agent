# Career-Alter-Ego-AI-Agent

**Career Alter Ego** is a personal AI chatbot designed to represent **Priyanshu Dwibedi** professionally.  
It uses **Google Gemini API (via OpenAI SDK)**, **Gradio** for chat UI, and **Pushover** for notifications.  

This assistant answers questions about Priyanshu’s **career, background, skills, and experience**,  
using data from a **LinkedIn PDF export** and a **professional summary**.  
It also records user contact details and logs unanswered questions for follow-up.

---

## 🚀 Features
- **Persona-based responses**: Always responds as *Priyanshu Dwibedi*.  
- **Smart tools**:
  - 📧 `record_user_details`: Records a user’s email, name, and notes.  
  - ❓ `record_unknown_question`: Logs unanswered questions.  
- **Real-time notifications**: Sends Pushover alerts for recorded details.  
- **Professional system prompt**: Keeps responses career-focused and engaging.  
- **Interactive chat UI**: Built with Gradio for a smooth user experience.  

---

## 🛠️ Tech Stack
- **Python 3.9+**
- [OpenAI SDK](https://pypi.org/project/openai/) (used with Google Gemini API)
- [Gradio](https://www.gradio.app/) – chat interface
- [dotenv](https://pypi.org/project/python-dotenv/) – environment variable management
- [pypdf](https://pypi.org/project/pypdf/) – extract text from LinkedIn PDF
- [requests](https://pypi.org/project/requests/) – push notifications via Pushover

├── me/
│ ├── linkedin.pdf # LinkedIn profile export (PDF)
│ └── summary.txt # Written career summary
├── main.py # Core chatbot implementation
├── .env # API keys & secrets
└── README.md # Documentation



---

## ⚙️ Setup & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/career-alter-ego.git
cd career-alter-ego
python -m venv .venv
source .venv/bin/activate   # Linux/Mac
.venv\Scripts\activate      # Windows
pip install -r requirements.txt


# Google Gemini API (via OpenAI SDK)
GOOGLE_API_KEY=your_gemini_api_key_here

# Pushover
PUSHOVER_TOKEN=your_pushover_app_token
PUSHOVER_USER=your_pushover_user_key


python main.py

---

## 📂 Project Structure


# Chatbot Application

Welcome! 👋  
This repository is a simple chatbot web application built with Flask and Hugging Face Transformers.

---

## About This Project

This project provides a conversational AI chatbot using the [facebook/blenderbot-400M-distill](https://huggingface.co/facebook/blenderbot-400M-distill) model.  
It features a web UI (leveraging templates from [ibm-developer-skills-network/LLM_application_chatbot](https://github.com/ibm-developer-skills-network/LLM_application_chatbot)) and a Flask backend that handles inference and conversation logic.

---

## Features

- **Conversational Memory:** Maintains context across turns during a session.
- **Modern LLM Backend:** Uses Hugging Face's Blenderbot 400M distilled model for responses.
- **Web Interface:** Clean, simple frontend for chatting with the bot.
- **CORS Enabled:** Backend supports cross-origin requests.
- **Modular:** Easy to swap models or adapt the front-end.

---

## File Structure

- `chatbot.py` — Main Flask application with chatbot logic.
- `templates/` — HTML templates for the web UI (from IBM's repo).
- `requirements.txt` — Python dependencies.

---

## Getting Started

### 1. Clone the Base Template

```bash
git clone https://github.com/ibm-developer-skills-network/LLM_application_chatbot
```

### 2. Install Requirements

```bash
python3.11 -m pip install -r LLM_application_chatbot/requirements.txt
```

### 3. Add Your Chatbot File

Replace or add your `chatbot.py` to the project root.

### 4. Run the Application

```bash
python3.11 chatbot.py
```

Then visit [http://localhost:5000](http://localhost:5000) in your browser.

---

## Notes & Limitations

- **Conversation Length:** The model may crash if the conversation history becomes too long. Consider limiting history for production use.
- **Model Download:** The first run will download the Blenderbot model from Hugging Face (~1GB).
- **Customization:** You can modify `chatbot.py` to use other models or add new features.

---

## Credits

- [AdityaK1301](https://github.com/AdityaK1301) — Project Author
- [IBM Developer Skills Network](https://github.com/ibm-developer-skills-network) — Source of web UI templates

---

# 🧠 AI Assistant with Long-Term Memory & Voice

![Project Status](https://img.shields.io/badge/Status-Production_Ready-success?style=for-the-badge)
![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)

**A secure, authenticated AI assistant built for speed and persistence.**

This application leverages **Groq's LPU inference engine** for lightning-fast responses, **LangChain** for orchestration, and a hybrid memory architecture using **Redis** (hot storage) and **MongoDB** (cold storage) to provide a seamless, context-aware conversational experience.

---

## 📸 Application Preview

### **Voice & Chat Interface**
*Speak naturally or type. The app transcribes voice instantly and responds with context.*

![Voice Interface](assets/Screenshot%202026-02-01%20232640.png)

### **Secure Login**
*User-isolated sessions ensure your chat history remains private.*

![Login Screen](assets/Screenshot%202026-02-01%20232542.png)

### **Memory & Settings Sidebar**
*Manage history, undo mistakes, and see your long-term memory bank in action.*

![Sidebar Memory](assets/Screenshot%202026-02-01%20232705.png)

---

## ✨ Key Features

| Feature | Description |
| :--- | :--- |
| **🔐 Secure Auth** | User registration & login with **bcrypt** password hashing and session management. |
| **🧠 Hybrid Memory** | **Redis** for instant context retrieval + **MongoDB Atlas** for permanent history storage. |
| **🎙️ Voice Input** | Real-time speech-to-text using **Groq Whisper** (Large V3 Turbo). |
| **💬 Smart Chat** | Streaming responses, undo functionality, and per-user isolated conversation history. |
| **⚡ Ultra-Fast** | Powered by **Groq's LLaMA 3** models for near-instant inference. |

---

## 🛠️ Tech Stack

### **Frontend**
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)

* **Chat UI**: Custom-styled chat interface.
* **Audio**: Native browser-based audio recording.

### **AI Core**
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=LangChain&logoColor=white) ![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logo=ai&logoColor=white)
* **Orchestration**: LangChain `ChatPromptTemplate` and `StrOutputParser`.
* **Inference**: Groq LPU (Language Processing Unit).
* **Speech**: Whisper V3 Turbo for transcription.

### **Data & Storage**
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
* **Redis (Upstash)**: Caching recent context window (Hot Memory).
* **MongoDB Atlas**: Persistent archival of all chats (Cold Storage).

---


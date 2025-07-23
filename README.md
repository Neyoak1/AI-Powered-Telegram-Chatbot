# Telegram Bot + Google Drive + Supabase Embeddings

<img width="960" height="505" alt="Screenshot 2025-06-21 002436" src="https://github.com/user-attachments/assets/67791636-a9cb-4f16-ad78-f9c369c3bc7a" />

---

## 📚 Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [How It Works](#how-it-works)
- [Use Case Ideas](#use-case-ideas)
- [How to Use](#how-to-use)
- [Contributing](#contributing)

---

## 🧠 Overview

This workflow enables a **chat interface on Telegram** that can:
- Accept messages and respond using an AI Agent.
- Extract and embed documents uploaded to **Google Drive**.
- Store and retrieve memory using **Supabase Vector Store**.
- Use **Google Gemini** for natural language understanding and context processing.

---

## 🚀 Key Features

- 🔁 Telegram AI chat loop
- 🧠 AI Agent with memory and tools
- 📄 Google Drive file triggers
- 🧮 Embedding pipeline (TXT & CSV support)
- 🧰 Supabase vector storage and lookup
- 🧩 Gemini-powered response generation

---

## 🛠 Tech Stack

- **n8n** – Workflow automation
- **Telegram Bot API** – Chat interface
- **Google Drive** – Document input
- **Google Gemini API** – AI chat + embeddings
- **Supabase** – Vector storage (via pgvector)
- **Markdown + CSV Parsing** – File support

---

## 🔄 How It Works

1. **Telegram Trigger** receives messages.
2. **AI Agent** queries memory (via Supabase) and tools (Google Gemini).
3. Responses are generated and sent back on Telegram.
4. Separately, files added to **Google Drive** trigger a parsing flow:
   - Files are read (TXT or CSV)
   - Text is split, embedded via Gemini
   - Stored in Supabase vector store
5. All context is reusable by the AI Agent in future chats.

---

## 💡 Use Case Ideas

- Chat with documents you upload  
- Sales or support bots that remember client history  
- AI-powered internal tools for teams  
- Knowledge base assistants for startups

---

## 🤝 Contributing

Pull requests and suggestions are welcome! Let's build better AI agents together.

---


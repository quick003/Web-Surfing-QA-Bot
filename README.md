# 🌍 Web-Surfing QA Bot

This is a **Colab-friendly, no-OpenAI-key** Question Answering bot that:
- Uses **SerpAPI** to search Google
- Scrapes and embeds top webpages
- Answers queries using **FLAN‑T5**, a lightweight open-source LLM
- Cites its sources with links

> ✅ No OpenAI API required  
> ✅ Free to use (100 SerpAPI searches/day)  
> ✅ Runs on CPU or GPU (Colab-supported)

---

## 🚀 Features

- 🔍 Google Search via [SerpAPI](https://serpapi.com)
- 🧠 Open-source LLM: `google/flan-t5-base`
- 🧱 Embeddings: `all-MiniLM-L6-v2` (fast + free)
- 🧰 Powered by LangChain RAG (Retrieval-Augmented Generation)
- 📜 Source citations included
- ⚡ Lightweight and runs in Colab with no local setup

---

## 📦 Requirements

- Python 3.8+
- [Google Colab](https://colab.research.google.com) (recommended)
- A free [SerpAPI key](https://serpapi.com/users/sign_up)

---

## 🔑 Setup

In Colab, before running the bot:

```python
import os, getpass
os.environ["SERPAPI_API_KEY"] = getpass.getpass("🔑 Enter SERPAPI_API_KEY: ")

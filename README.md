# 📚 AI-Powered Book Insight Platform

A full-stack web application that uses **AI + RAG (Retrieval-Augmented Generation)** to provide intelligent insights and question-answering over book data.

---

## 🚀 Features

* 📖 Automated book data scraping
* 🧠 AI-generated book summaries
* 🎯 Genre classification (AI-based)
* 🔍 Recommendation system (similar books)
* 💬 RAG-based Question Answering with context
* 🔗 REST APIs using Django REST Framework
* 🎨 Interactive frontend built with React + Tailwind CSS

---

## 🏗️ Tech Stack

### Backend

* Python
* Django REST Framework
* MySQL (or SQLite)
* ChromaDB (Vector Database)
* Sentence Transformers (Embeddings)
* OpenAI API / LM Studio (LLM)

### Frontend

* ReactJS
* Tailwind CSS
* Axios

### Automation

* Selenium / BeautifulSoup

---

## 📂 Project Structure

```
book-ai-platform/
│
├── backend/
├── frontend/
├── docs/
├── samples/
├── README.md
```

---

## ⚙️ Setup Instructions

### 🔹 Backend Setup

```bash
cd backend
python -m venv venv
venv\Scripts\activate   # (Windows)
pip install -r requirements.txt

python manage.py migrate
python manage.py runserver
```

---

### 🔹 Frontend Setup

```bash
cd frontend
npm install
npm start
```

---

## 🔌 API Endpoints

### 📥 GET APIs

* `/books/` → List all books
* `/books/<id>/` → Get book details
* `/books/recommend/` → Get recommended books

### 📤 POST APIs

* `/books/upload/` → Scrape & upload books
* `/books/ask/` → Ask questions (RAG pipeline)

---

## 🧠 RAG Pipeline Flow

1. Convert book descriptions into embeddings
2. Store embeddings in ChromaDB
3. Convert user question into embedding
4. Perform similarity search
5. Retrieve relevant chunks
6. Send context + question to LLM
7. Return answer with sources

---

## 🧪 Sample Questions

* "What is this book about?"
* "Recommend books similar to this"
* "Summarize this book"

---

## 📸 Screenshots

> Add your UI screenshots here (Dashboard, Q&A, Book Detail Page)

---

## 📦 Sample Data

Check `/samples/` folder for:

* Sample books JSON
* Sample questions

---

## ✨ Bonus Features (Optional)

* Caching AI responses
* Async scraping (Celery)
* Chat history
* Advanced chunking strategies

---

## 📊 Evaluation Criteria Covered

* ✅ Functional RAG pipeline
* ✅ Clean and modular code
* ✅ Responsive UI
* ✅ AI-based insights

---

## 👨‍💻 Author

Your Name

---

## 📌 Notes

* Add your OpenAI API key in `.env`
* Ensure backend runs before frontend
* Early submission improves chances 🚀

---

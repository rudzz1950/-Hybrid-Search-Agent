# Contextual Personal Assistant with Hybrid Search

This project implements a lightweight conversational agent that answers user queries using:
- **Static knowledge** from a PDF or text document
- **Simulated memory** from previous user interactions
- **Cosine similarity-based retrieval** over embedded document chunks
- **Natural language generation** using OpenAI's GPT-3.5-turbo

---

## 💡 Features
- Embeds PDF content using Sentence Transformers (`all-MiniLM-L6-v2`)
- Retrieves top-k relevant chunks using cosine similarity
- Merges current query with chat history and document context
- Generates helpful, context-aware answers
- Includes fallback rule-based response if OpenAI API fails

---

## 🛠 How to Run

1. Place a PDF file named `movie_script.pdf` in the same directory.
2. (Optional) Create `memory.json` to simulate past interactions.
3. Install dependencies:

```bash
pip install openai sentence-transformers PyPDF2 torch

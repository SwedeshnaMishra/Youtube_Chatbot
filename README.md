# 🎥 YouTube Video Q&A with RAG (Retrieval-Augmented Generation)

An AI-powered project that allows users to ask questions about any YouTube video using its transcript.  
Built using **Python, LangChain, FAISS, Hugging Face Transformers, and YouTube Transcript API**.

The system extracts captions from a YouTube video, converts them into searchable embeddings, stores them in a vector database, retrieves relevant transcript chunks, and generates accurate answers from context.

---

## 🚀 Key Features

1. **📺 YouTube Transcript Extraction**  
   Automatically fetch transcript/captions from YouTube videos using video ID.

2. **✂️ Smart Text Chunking**  
   Splits long transcripts into manageable chunks for efficient retrieval.

3. **🧠 Embedding Generation**  
   Converts transcript chunks into vector embeddings using Hugging Face models.

4. **📦 FAISS Vector Store**  
   Stores embeddings for fast semantic similarity search.

5. **🔍 Context Retrieval**  
   Retrieves most relevant transcript chunks based on user questions.

6. **🤖 AI Answer Generation**  
   Uses Hugging Face FLAN-T5 model to answer questions from retrieved context only.

7. **⚡ Fully Local / Free Option**  
   No paid API required (works with open-source Hugging Face models).

8. **📓 Jupyter Notebook Friendly**  
   Easy to run and demonstrate in VS Code / Jupyter Notebook.

---

## 📁 Project Structure

```text
YouTube-RAG-QA/
│── youtube_rag.ipynb
│── requirements.txt
│── README.md
```

---

## ⚙️ Tech Stack

| Component      | Technology                     |
|------------|--------------------------------|
| Language   | Python  |
| Transcript API    | youtube-transcript-api  |
| Embeddings  | Langchain                        |
| Vector Database | FAISS |
| LLM       | Google FLAN-T5 (Hugging Face)   |
| Environment | Jupyter Notebook / VS Code |

---

## 🛠 Setup Instructions

### Install Dependencies

```bash
pip install langchain
pip install langchain-community
pip install transformers
pip install sentence-transformers
pip install faiss-cpu
pip install youtube-transcript-api
pip install torch
```

---

## ▶️ Run Project

1. Open Jupyter Notebook / VS Code
2. Run all notebook cells in order
3. Enter YouTube video ID
4. Ask questions related to the video transcript

---

## 📍 Example Workflow

- Provide YouTube video ID
- Transcript gets extracted automatically
- Transcript converted into chunks
- Chunks embedded and stored in FAISS
- Ask question like:
  ```bash
  Is nuclear fusion discussed in this video ?
  ```
- AI returns context-aware answer

---

## 💡 Example Use Cases

- Summarize long podcasts
- Learn from educational videos
- Search interview discussions
- Extract key points from lectures
- Ask questions from conference talks

---

## 🔮 Future Improvements

- Add Streamlit / Flask UI
- Support PDF + YouTube together
- Multi-video search
- Chat history memory
- Better open-source LLM integration

---

## For Contributing
If you want to contribute to this project, please follow these steps:
- `Fork` the repository.
- Create a new branch `(git checkout -b feature/your-feature-name)`.
- Make your changes and commit them `(git commit -m 'Add some feature')`.
- Push to the branch `(git push origin feature/your-feature-name)`.
- Open a pull request.

---

## Project Maintainer
**Github:** [Swedeshna Mishra](https://github.com/SwedeshnaMishra)

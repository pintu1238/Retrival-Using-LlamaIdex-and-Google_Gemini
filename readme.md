# 📄 Information Retrieval System using LlamaIndex & Google Gemini

## 🚀 Project Overview

This project is an **AI-powered Question Answering (QA) System** built using **LlamaIndex** and **Google Gemini**.
It enables users to interact with their own documents (PDFs, text files, etc.) and get **accurate, context-aware answers**.

The system follows a **Retrieval-Augmented Generation (RAG)** approach, where relevant information is first retrieved from documents and then passed to a Large Language Model (Gemini) to generate a precise response.

---

## 🧠 Key Features

* 📂 Load and process documents from local directories
* 🔍 Semantic search using embeddings
* ⚡ Fast and efficient information retrieval
* 🤖 AI-powered answer generation using Google Gemini
* 💾 Persistent storage of index for faster reuse
* 🔄 Scalable architecture for large datasets

---

## 🏗️ Architecture (RAG Pipeline)

The system works in the following steps:

1. **Document Loading**
   Documents are loaded using LlamaIndex.

2. **Chunking**
   Large documents are split into smaller chunks.

3. **Embedding Generation**
   Each chunk is converted into vector embeddings.

4. **Vector Index Creation**
   All embeddings are stored in a vector index.

5. **Query Processing**

   * User query is converted into embedding
   * Relevant chunks are retrieved

6. **Answer Generation**
   Retrieved context + query → Gemini → Final Answer

---

## 🛠️ Tech Stack

* **LlamaIndex** – Data indexing & retrieval
* **Google Gemini** – LLM for answer generation
* **HuggingFace Embeddings** – Vector representation
* **Python** – Core programming language
* **Streamlit (optional)** – UI interface

---

## 📁 Project Structure

```
QA System/
│── data/                # Input documents
│── notebook/            # Experiment notebooks
│── streamlit.py         # UI (if used)
│── requirements.txt     # Dependencies
│── logger.py            # Logging utility
│── exception.py         # Exception handling
│── template.py          # Base structure
│── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/Information-Retrieval-Using-LlamaIndex-Gemini.git
cd QA-System
```

### 2️⃣ Create Environment

```bash
conda create -n qa_system python=3.11
conda activate qa_system
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Set API Key

Create a `.env` file and add:

```
GOOGLE_API_KEY=your_api_key_here
```

---

## ▶️ Run the Project

```bash
python main.py
```

Or (if using Streamlit):

```bash
streamlit run streamlit.py
```

---

## 💡 Example Use Case

* Ask: *"What is Machine Learning?"*
* System retrieves relevant document chunks
* Gemini generates a structured answer

---

## 📊 Applications

* 📚 Chat with PDFs
* 🧾 Resume Analyzer
* 🏢 Company Knowledge Base
* 📖 Research Assistant
* 🤖 AI Chatbot with custom data

---

## ⚠️ Challenges Faced

* Gemini embedding model compatibility issues
* Environment and dependency conflicts
* API version changes

---

## 🔮 Future Improvements

* Add real-time chat UI
* Integrate vector databases (FAISS, Pinecone)
* Add multi-document support
* Improve response accuracy with reranking

---

## 👨‍💻 Author

**Vicky (Pintu)**
Aspiring Data Engineer | AI Enthusiast

---

## ⭐ Conclusion

This project demonstrates how modern AI systems combine **retrieval + generation** to create powerful, scalable applications.
It is a strong foundation for building **real-world AI products** like chatbots, assistants, and enterprise knowledge systems.

---

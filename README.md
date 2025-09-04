# 🎥 AI-Powered YouTube Summarizer & QA Tool with RAG, LangChain, FAISS  

## 📌 Overview  
This project is an **AI-powered Question Answering (QA) tool** that extracts and summarizes information from **YouTube videos**.  
By leveraging **LangChain**, **FAISS**, and a **Large Language Model (LLM)**, the system enables:  
- Automatic transcript extraction from YouTube videos.  
- Summarization of long transcripts into concise overviews.  
- **Retrieval-Augmented Generation (RAG)** for answering user queries based on video content.  
- A **Gradio-powered interface** for interactive and user-friendly exploration.  

With the explosion of online video content, manually searching through lengthy footage is inefficient. This tool automates the process, turning **dense transcripts into summaries** and enabling **precise video segment retrieval** using FAISS embeddings.  

---

## 🚀 Features  
- 🔎 **Transcript Extraction** – Fetches and processes YouTube transcripts.  
- ✂️ **Summarization** – Converts long transcripts into concise, human-readable summaries.  
- 🤖 **Question Answering (RAG)** – Uses embeddings + FAISS retriever to answer user questions.  
- 📚 **Embeddings** – Supports Hugging Face embeddings (`all-MiniLM-L6-v2`).  
- ⚡ **Vector Search with FAISS** – Enables semantic search over video content.  
- 🎛️ **Interactive Gradio UI** – Simple and intuitive web interface for users.  

---

## 🏗️ Architecture  
1. **Transcript Loader** → Extract transcript text from YouTube.  
2. **Text Processing** → Chunking & preprocessing for embeddings.  
3. **Embedding Model** → Converts text chunks into vector embeddings.  
4. **FAISS Vector Store** → Stores and retrieves embeddings efficiently.  
5. **Retriever + LLM** → Retrieves relevant chunks and generates answers (RAG).  
6. **Gradio App** → Provides a web-based interactive interface.  

---

## 🛠️ Installation  

### 1. Clone the repository  

gh repo clone pradeep-mahat0/AI-Powered-YouTube-Summarizer-QA-Tool
cd AI-Powered-YouTube-Summarizer-QA-Tool

### 2. Create a virtual environment

python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

### 3. Install dependencies

pip install -r requirements.txt

### 4. Set up Hugging Face API token

Create a free token from Hugging Face
 and set it:

Make a .env file and store your api-key like this:
HUGGINGFACEHUB_API_TOKEN="your_token_here"

## ▶️ Usage
### Run the application with:
python ytbot.py

### This will launch a Gradio interface at:
http://localhost:7860

### Here how it looks-->

<img width="1827" height="975" alt="Screenshot 2025-09-04 101446" src="https://github.com/user-attachments/assets/080977b0-2a7b-4f7a-bfc7-230c36f33b29" />

### Paste your YouTube vedio link -->sample example (https://www.youtube.com/watch?v=5MuIMqhT8DM)

### Click on the Summarize vedio button

<img width="1678" height="611" alt="Screenshot 2025-09-04 100754" src="https://github.com/user-attachments/assets/ed3be3f1-e7a4-4e59-90b8-8d393475c52e" />

### Ask question related to vedio and click on the ask a question button

<img width="1631" height="1022" alt="Screenshot 2025-09-04 100814" src="https://github.com/user-attachments/assets/da10224e-b8e7-40b1-a621-692d24698657" />

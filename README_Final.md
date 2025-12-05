# YouTube RAG Career Bot – Final Bootcamp Project

## 🚀 Overview
This repository contains our final Bootcamp project: a fully functional **Retrieval-Augmented Generation (RAG)** system built around YouTube career-related videos.  
The system retrieves transcripts, chunkifies, embeds and stores them in a vector database and uses a custom RAG pipeline + agent to answer questions with great accuracy. 

---

## 🎯 Project Goals
- Learn how to build an end‑to‑end RAG pipeline  
- Understand vector databases and semantic search  
- Integrate LLMs with tool calling  
- Add audio capabilities (Whisper + TTS)  
- Build a user-friendly interface (Gradio)  
- Evaluate RAG responses with BLEU, ROUGE-L, and cosine similarity  

---

## 🧱 Features
- **YouTube transcript ingestion** (API + local fallback)
- **Chunking & metadata processing**
- **Embeddings via OpenAI models**
- **Chroma vector database**
- **Custom RAG query pipeline**
- **LLM agent with tools & memory**
- **Speech-to-Text (Whisper)**
- **Text-to-Speech (TTS)**
- **Gradio UI (Text + Audio)**
- **Evaluation metrics: BLEU, ROUGE-L, semantic similarity**

---

## 🏗 Architecture Diagram
![Architecture Diagram](A_flowchart_diagram_in_the_image_illustrates_a_Ret.png)

## 🚀 Setup Guide

### ⚙️ 1. Clone the Repository
```bash
git clone <your-repo-url>
cd <your-repo-folder>
```

### 📦 2. Install Required Packages  
```bash
pip install -r requirements.txt
```

### 🔐 3. Add OpenAI API Key  
Create a `.env` file:
```
OPENAI_API_KEY=your_api_key_here
```

You may rename `.env.example` → `.env`.

### 🎬 4. Add YouTube URLs  
Inside the notebook:
```python
youtube_urls = [
    "https://youtube.com/watch?v=....",
]
```
### 🧠 6. Run the Notebook

### 🖥 5. Launch Gradio Interface  
```python
demo.launch(share=True)
```

---

## 🖥 User Interface (Gradio)

### **Text Chat**
- Ask questions about the indexed YouTube videos  
- Bot answers using the RAG pipeline  
- Personality + memory system included  

### **Audio Question**
- Record audio  
- Whisper transcribes  
- Bot answers in text and optioally via audio

---

## 📊 Evaluation Metrics
To test the quality of generated answers, we implemented:

- **Cosine Similarity** (semantic closeness)  
- **BLEU Score** (phrase overlap)  
- **ROUGE-L Score** (summary-style match)  

These help measure whether the system understands and retrieves relevant content.

---

## 🔧 Tech Stack
- **Python**
- **LangChain**
- **OpenAI API**
- **ChromaDB**
- **YouTube Transcript API**
- **Whisper (Speech-to-Text)**
- **TTS (Text-to-Speech)**
- **Gradio**
- **Pandas, NumPy**

---

## Final Notes
In the final project, we archieved and learned the following:
- Built a RAG system that queries YouTube transcripts for answers.
- Retrieved and cleaned video transcripts automatically.
- Created text chunks and stored them in a vector database for retrieval.
- Used LangChain agents, tools, and memory to coordinate tasks.
- Designed prompts and a persona to guide the AI's behavior.
- Integrated speech-to-text and text-to-speech for audio interaction.
- Built a Gradio interface for text and voice chatting.
- Evaluated answers visually and then tested with BLEU, ROUGE-L, and semantic similarity.
- Used LangSmith to test, trace, and debug outputs.
- Learned trade-offs in accuracy, speed, and creativity.
- Gained practice with real-world data pipelines and API integrations.

---


## 📜 License
This project is intended for educational use only.


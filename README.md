# Retrieval-Augmented Generation (RAG) Chatbot with LLaMA3 and Groq

This project implements a **Retrieval-Augmented Generation (RAG) chatbot** that can answer user queries by retrieving context from both **PDF documents** and **web sources**, and then generating precise responses using **Groq LLMs**.

## 🚀 Features
- Ingests and processes **PDF files** and **webpages**.
- Splits text into chunks and stores embeddings in a **FAISS vector database**.
- Uses **Groq-hosted LLaMA3/Mixtral models** for context-aware response generation.
- Interactive **Streamlit web app** with a natural language interface.
- Includes **document similarity search** for transparency.

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Frameworks & Libraries:** Streamlit, LangChain, FAISS, OpenAI/Ollama Embeddings, Groq LLMs  
- **Deployment:** Local with Streamlit  
- **Environment Variables:** Stored securely in `.env`  

## 📂 Project Structure
.
├── llama3.py # PDF-based RAG chatbot
├── app.py # Web-based RAG chatbot
├── requirements.txt # Dependencies
├── .env # API keys (not included in repo)
└── README.md


## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/rag-llama3-groq.git
   cd rag-llama3-groq
2. **Create a virtual environment (recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # Mac/Linux
   venv\Scripts\activate      # Windows
3. **Install dependencies**
    ```bash 
    pip install -r requirements.txt
4. **Set up environment variables**
Create a .env file in the project root:
   ```bash
      env
      GROQ_API_KEY=your_groq_api_key
      OPENAI_API_KEY=your_openai_api_key

5.**Run the app**
   - For Web-based RAG:
      ```bash
         streamlit run app.py
   
  - For PDF-based RAG:
      ```bash
         streamlit run llama3.py



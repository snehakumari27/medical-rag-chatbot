# 🩺 Medical RAG Chatbot

A Medical Question-Answering chatbot built using **Retrieval-Augmented Generation (RAG)**.  
The system retrieves relevant information from a medical knowledge base and uses a Large Language Model (LLM) to generate contextual responses.

The project combines **LangChain, FAISS, Hugging Face embeddings, Groq LLM, and Streamlit** to provide an interactive chatbot interface.

---

## 📌 Project Overview

Medical information can be large and difficult to search manually. This project uses a Retrieval-Augmented Generation approach to retrieve relevant information from a knowledge base before generating an answer.

Instead of relying only on the LLM's internal knowledge, the chatbot first searches the stored medical documents and then uses the retrieved context to generate a response.

### Main Workflow

```text
Medical Documents
       ↓
Document Processing
       ↓
Text Embeddings
       ↓
FAISS Vector Database
       ↓
User Question
       ↓
Similarity Search
       ↓
Relevant Documents
       ↓
Prompt + Retrieved Context
       ↓
Groq LLM
       ↓
Generated Response
       ↓
Streamlit Chat Interface


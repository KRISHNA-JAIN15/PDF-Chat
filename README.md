# PDF-Chat

## Chat with PDF using RAG and Google Generative AI

### 📜 Project Description

This project allows users to interact with uploaded PDF files using **Retrieval-Augmented Generation (RAG)** and **Google Generative AI**. The application extracts text from PDFs, splits the text into chunks, stores embeddings in a FAISS vector store, and provides answers to user queries by retrieving relevant context from the documents.

Key features:
- Upload multiple PDF files and process them.
- Ask questions about the content of the uploaded PDFs.
- Get detailed answers with relevant context from the PDFs.
- Powered by Google Generative AI and FAISS for embeddings and vector storage.

---

## 🛠 Dependencies

The project uses the following dependencies:

- **Streamlit**: For building the web interface.
- **PyPDF2**: For extracting text from PDF files.
- **LangChain**: For building the RAG pipeline.
- **langchain_community.vectorstores**: For FAISS vector store.
- **Google Generative AI**: For embeddings and conversational responses.
- **Python-dotenv**: For managing API keys securely.

Install the required dependencies:

```bash
pip install streamlit PyPDF2 langchain langchain-community faiss-cpu google-generativeai python-dotenv

```

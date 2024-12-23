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

## 🚀 How to Run the App
1. Clone the Repository:
   ```bash
   git clone https://github.com/your-username/chat-with-pdf.git
   cd chat-with-pdf
   ```
2. Add Your Google API Key:
   Create a .env file in the root directory.
   Add your API key:
    ```bash
    GOOGLE_API_KEY=your_google_api_key
    ```
3. Run the Application:
   ```bash
   streamlit run app.py
   ```
4. Open your browser and go to http://localhost:8501.

## Project Structure 

```bash
.
├── app.py               # Main application file
├── requirements.txt     # List of dependencies
├── .env                 # API key file (not committed to version control)
└── README.md            # Project documentation
```

## 📖 How It Works
1. Upload PDFs: Users can upload multiple PDFs via the sidebar.

2. Text Processing: The text is extracted from PDFs using PyPDF2.
The extracted text is split into manageable chunks using RecursiveCharacterTextSplitter.

3. Embedding Creation: Text chunks are converted into embeddings using Google Generative AI Embeddings.
These embeddings are stored in a FAISS vector store for efficient retrieval.

4. Ask Questions: Users input their questions in the main interface.
Relevant context is retrieved from the vector store using similarity search.

5. Retrieve and Answer: A detailed and contextually relevant answer is generated using Google Generative AI.

   

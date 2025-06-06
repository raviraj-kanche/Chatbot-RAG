# DMCLI Chatbot 🤖

DMCLI Chatbot is a PDF-based question-answering system built with Streamlit and powered by Google's Generative AI. It allows users to upload PDF documents, process them, and ask questions based on the content of those documents.

## Features

- PDF upload and processing
- Text extraction from PDFs
- Text chunking for efficient processing
- Vector store creation using FAISS for similarity search
- Conversational AI using Google's Generative AI model
- User-friendly interface built with Streamlit

## Requirements

The project requires the following Python packages:

- streamlit
- google-generativeai
- python-dotenv
- langchain
- PyPDF2
- faiss-cpu
- langchain_google_genai
- langchain-community

You can install these dependencies using the provided `requirements.txt` file:

```
pip install -r requirements.txt
```

## Usage

1. Run the Streamlit app:
   ```
   streamlit run chatbot.py
   ```

2. Enter your Google Gemini API key when prompted.

3. Upload PDF files using the sidebar.

4. Click the "Submit & Process" button to extract text from the PDFs and create the vector store.

5. Ask questions in the main input field, and the chatbot will provide answers based on the content of the uploaded PDFs.

## How it Works

1. The app extracts text from uploaded PDF files.
2. The extracted text is split into smaller chunks for efficient processing.
3. These text chunks are converted into vector embeddings using Google's AI model.
4. The embeddings are stored in a FAISS index for fast similarity search.
5. When a user asks a question, the app searches for the most relevant text chunks.
6. The relevant chunks are used as context for the AI model to generate an answer.

## Note

This project requires a Google Gemini API key to function. Make sure you have a valid API key before running the application.

## License

[Add your chosen license here].

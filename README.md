# RAG (Retrieval-Augmented Generation) Question Answering System

## Project Overview
This project implements a sophisticated question-answering system using the Retrieval-Augmented Generation (RAG) approach, 
combining the power of language models with document retrieval. The system is designed to provide clear and concise answers to user queries, 
regardless of whether the input is text or code. It is particularly adept at processing PDF documents, extracting their contents, and using the extracted text to generate relevant responses.

## Key Features
- **Document Handling**: Ability to process PDF documents to extract text.
- **Retrieval-Augmented Answering**: Uses a combination of FAISS vector storage for efficient retrieval and OpenAI's language models for generating answers.
- **Streamlit Interface**: Includes a user-friendly web interface built with Streamlit, allowing users to interact with the system by submitting questions and uploading documents directly.

## Technologies Used
- **Python**: The primary programming language.
- **Streamlit**: For building the interactive web application.
- **Langchain**: Utilized for building the logic chains and prompt templates for the language model.
- **OpenAI's GPT Models**: For generating text responses.
- **FAISS**: For efficient similarity search and retrieval of documents.
- **PyPDF2**: For extracting text from PDF files.

## Installation
To set up this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd RAG
    ```

2. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Streamlit application:
    ```bash
    streamlit run RAG.py
    ```

## Usage
After installation, you can run the system via Streamlit. It will prompt you to enter text or upload a PDF document for analysis. The system will process the input and return an answer based on the content it retrieves and the questions asked.

## How It Works
- **Document Upload and Text Extraction**: Users can upload PDF documents, from which text is extracted.
- **Text Chunking**: The extracted text is chunked for better management and processing.
- **Vector Store Creation**: Text chunks are converted into vector representations using OpenAI's embeddings.
- **Question Answering**: Combines retrieved document information with the generative capabilities of OpenAI's models to answer questions.

## Contributing
Contributions to this project are welcome! Please fork the repository, make your changes, and submit a pull request.

## Acknowledgments
Thanks to everyone who has contributed to the development and testing of this innovative question-answering system.


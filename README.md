# Chat with PDF

This is a Streamlit web application that allows users to ask questions based on the content of uploaded PDF files. The application utilizes language processing and conversational AI techniques to generate responses to user queries.

## Features

- Users can upload one or multiple PDF files.
- The application extracts text from the PDF files and divides it into manageable chunks for processing.
- The extracted text is indexed using Google Generative AI Embeddings and stored in a vector store for efficient retrieval.
- Users can input questions related to the content of the PDF files.
- The application retrieves relevant text chunks based on the user's question using FAISS (Facebook AI Similarity Search).
- The retrieved text chunks are fed into a conversational AI model (Gemini Pro) for generating responses to the user's questions.
- Responses are displayed to the user in real-time.

## Requirements

- Python 3.x
- Streamlit
- PyPDF2
- langchain
- langchain_google_genai
- langchain_community
- FAISS
- Google Generative AI

## Installation

1. Clone the repository:

git clone <repository_url>

2. Install dependencies:

pip install -r requirements.txt

3. Set up environment variables:

   Create a `.env` file in the root directory of the project and add your Google API key:

GOOGLE_API_KEY=<your_google_api_key>

4. Run the application:

streamlit run app.py

## Usage

1. Access the application via the URL provided after running the `streamlit run` command.
2. Upload one or multiple PDF files using the file uploader.
3. Click on the "Submit & Process" button to extract text from the PDF files and index it.
4. Enter a question related to the content of the PDF files in the text input field.
5. Press Enter or click outside the text input field to submit the question.
6. View the generated response below the text input field.

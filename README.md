# Chat with PDF 💁🔍📚
This project allows users to upload PDF files and interact with their content using natural language questions. By leveraging LangChain and Google Generative AI, this application processes the PDFs, creates embeddings, and performs conversational queries to provide accurate responses from the PDF content.

## Features
Upload PDF Files: Users can upload multiple PDF files.
Process PDF Content: Extract text from uploaded PDFs and split it into manageable chunks.
Generate Embeddings: Create vector embeddings using Google Generative AI for the text chunks.
Store Embeddings: Store the embeddings locally using FAISS (Facebook AI Similarity Search).
Conversational Interface: Interact with the PDF content through natural language questions and get detailed answers.
Getting Started
Prerequisites
Python 3.7+
Streamlit
PyPDF2
LangChain
FAISS
Google Generative AI
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/Nikk1412/Chat-with-PDF.git
cd chat-with-pdf
Create a virtual environment and activate it:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Set up your Google API Key:

Create a .env file in the root directory.

Add your Google API key to the .env file:

makefile
Copy code
GOOGLE_API_KEY=your_google_api_key
Running the Application
Run the Streamlit application:

bash
Copy code
streamlit run app.py
Open your web browser and go to http://localhost:8501 to use the application.

Usage
Upload PDF Files: Use the sidebar to upload one or more PDF files.
Process PDFs: Click on the "Submit & Process" button to extract and process the text from the uploaded PDFs.
Ask Questions: Enter your questions in the input box and get detailed answers based on the PDF content.
How It Works
PDF Text Extraction: The application reads the text from each page of the uploaded PDFs.
Text Chunking: The extracted text is split into chunks to make it manageable for processing.
Embedding Generation: Each text chunk is converted into a vector embedding using Google Generative AI.
Vector Storage: The embeddings are stored locally using FAISS for efficient similarity search.
Conversational Query: When a user asks a question, the application retrieves the most relevant text chunks and generates a detailed response using the pre-defined prompt template and Google Generative AI.
Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue.

License
This project is licensed under the MIT License.

Acknowledgments
LangChain
Google Generative AI
FAISS
Streamlit
PyPDF2

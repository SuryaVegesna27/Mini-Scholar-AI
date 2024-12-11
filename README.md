# Mini Scholar AI

Mini Scholar AI is an AI-powered platform designed to simplify academic research by enabling efficient text extraction, semantic search, and summarization of research papers. It leverages state-of-the-art NLP technologies like Sentence Transformers, ChromaDB, and ChatGPT API to deliver contextual insights and enhance productivity.

# Features

Text Extraction: Extracts text from PDFs for processing.

Semantic Search: Retrieves contextually relevant information using Sentence Transformers and ChromaDB.

Summarization: Summarizes research papers to provide quick insights.

Interactive Q&A: Uses ChatGPT API for contextual question-answering.

Keyword Search: Locates documents based on user-provided keywords.

User-Friendly Interface: Built with Streamlit for an intuitive experience.

# Technologies Used

Programming Language: Python

Libraries:

PyPDF2: For extracting text from PDFs.

Sentence Transformers: For generating semantic embeddings.

ChromaDB: For storing embeddings and metadata.
ChatGPT API: For generating contextual answers and summaries.
BeautifulSoup: For web scraping research papers.
Streamlit: For building an interactive user interface.
Ngrok: For deploying the app to a public URL.
Prerequisites
Before running the project, ensure you have the following installed:

Python 3.8 or above.
Required Python libraries:
bash
Copy code
pip install pypdf2 sentence-transformers chromadb streamlit openai beautifulsoup4
An OpenAI API key to use the ChatGPT API.
Setup and Configuration
1. Clone the Repository
bash
Copy code
git clone https://github.com/SuryaVegesna27/Machine-Learning.git
cd Machine-Learning
2. Set Up OpenAI API Key
Create an .env file in the project directory and add your OpenAI API key:
bash
Copy code
OPENAI_API_KEY=your_openai_api_key
3. Install Dependencies
Install all required libraries using the provided requirements.txt:

bash
Copy code
pip install -r requirements.txt
4. Configure Google Drive Integration (Optional)
If you want to save processed files and embeddings to Google Drive, mount your Google Drive using PyDrive or equivalent tools.

How to Run
1. Start the Streamlit App
Run the Streamlit application locally:

bash
Copy code
streamlit run app.py
This will start the app on http://localhost:8501.

2. Expose the App to the Internet
Use Ngrok to make the app accessible online:

bash
Copy code
ngrok http 8501
Ngrok will provide a public URL like https://your_ngrok_url.ngrok.io.

Usage Instructions
1. Upload PDFs
Navigate to the upload section of the app.
Upload your research PDFs for processing.
2. Semantic Search
Enter a query in natural language.
The system retrieves the top 3 relevant text chunks with context.
3. Q&A
Type a question related to the uploaded PDFs.
The app uses the ChatGPT API to generate an answer with cited sources.
4. Summarization
Select a document to summarize.
View a concise summary generated by the ChatGPT API.
5. Keyword Search
Input a keyword to locate relevant documents.
Results are displayed with metadata for easy navigation.
Results and Outputs
Semantic Search: Top 3 relevant chunks with metadata (e.g., file name, chunk ID).
Q&A: Precise answers generated by ChatGPT.
Summarization: A concise summary of the selected document.
Keyword Search: List of matching documents and details.
Future Enhancements
Support for multilingual document processing.
Real-time updates for new PDFs.
Advanced filtering by metadata (e.g., author, publication year).
Scalable architecture for handling large datasets.

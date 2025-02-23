# MedicalBot
MedicalBot is an AI-powered chatbot designed to assist with medical inquiries by retrieving relevant information from a vast collection of medical texts. It utilizes retrieval-augmented generation (RAG) to enhance response accuracy.

## Features
- **Medical Document Parsing:** Extracts structured data from medical PDFs using PyPDF.

- **Text Chunking:** Splits documents into smaller, meaningful chunks for better retrieval accuracy.

- **Embedding Generation:** Converts text chunks into numerical embeddings using sentence-transformers from Hugging Face.

- **Vector Database (Pinecone on AWS):** Stores embeddings in Pinecone for efficient similarity searches.

- **Query Processing:** Uses cosine similarity to match user queries with relevant document chunks.

- **Context Retrieval:** Fetches the most relevant text chunks based on query relevance.

- **LLM Response Generation (OpenAI API):** Generates responses using OpenAI’s model with retrieved context.

- **Interactive UI:** Built with FastAPI and designed using HTML, CSS, and Bootstrap for a smooth user experience.

- **Deployment:** Runs locally for development with embeddings stored on AWS Pinecone.

- **User Interaction:** Handles user queries, retrieves relevant data, and displays responses dynamically.

## Tech Stack
- **Frontend:** FastAPI, HTML, CSS, Bootstrap

- **Backend:** Python (FastAPI)

- **Vector Database:** Pinecone (hosted on AWS)

- **Embedding Model:** Sentence-Transformers (Hugging Face)

- **LLM:** OpenAI API

## Screenshots
![](https://github.com/GauravAnand30/MedicalBot/blob/main/screen%20shot/Screenshot%202025-02-24%20004028.png)
![]


## Installation
- **Clone the repository:**

## bash
Copy
```sh
git clone REPO_LINK
cd REPO_NAME
Create a Virtual Environment:

bash
Copy
python -m venv env
Activate Virtual Environment:

On Windows:

bash
Copy
env\Scripts\activate
On macOS/Linux:

bash
Copy
source env/bin/activate
Install Dependencies:

bash
Copy
pip install -r requirements.txt
Create Pinecone Database:

Set up an account on Pinecone.

Create an index for storing embeddings.

Add your Pinecone API key to the environment variables or configuration file.

Run Index Storage Script:

bash
Copy
python store_index.py
Start the Application:

bash
Copy
python app.py
Now, you can access the application on http://localhost:8000/ 🎯.#

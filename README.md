# Medical RAG Q&A
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


# Medical RAG Q&A

MedicalBot is an AI-powered chatbot designed to assist with medical inquiries by retrieving relevant information from a vast collection of medical texts. It utilizes **Retrieval-Augmented Generation (RAG)** to enhance response accuracy, ensuring users receive precise and contextually relevant medical information.

## 🚀 Features

- **📄 Medical Document Parsing:** Extracts structured data from medical PDFs using PyPDF.
- **🔗 Text Chunking:** Splits documents into smaller, meaningful chunks for better retrieval accuracy.
- **📊 Embedding Generation:** Converts text chunks into numerical embeddings using `sentence-transformers` from Hugging Face.
- **🗄️ Vector Database (Pinecone on AWS):** Stores embeddings in **Pinecone** for efficient similarity searches.
- **🔎 Query Processing:** Uses cosine similarity to match user queries with relevant document chunks.
- **📚 Context Retrieval:** Fetches the most relevant text chunks based on query relevance.
- **🤖 LLM Response Generation (OpenAI API):** Generates responses using OpenAI’s model with retrieved context.
- **🎨 Interactive UI:** Built with FastAPI and designed using **HTML, CSS, and Bootstrap** for a smooth user experience.
- **🚀 Deployment:** Runs locally for development with embeddings stored on **AWS Pinecone**.
- **🗣️ User Interaction:** Handles user queries, retrieves relevant data, and dynamically displays responses.

## 🛠️ Tech Stack

- **Frontend:** FastAPI, HTML, CSS, Bootstrap
- **Backend:** Python (FastAPI)
- **Vector Database:** Pinecone (hosted on AWS)
- **Embedding Model:** `sentence-transformers` (Hugging Face)
- **LLM:** OpenAI API

## 📸 Screenshots

![Screenshot 1](https://github.com/GauravAnand30/MedicalBot/blob/main/screen%20shot/Screenshot%202025-02-24%20004028.png)
![Screenshot 2](https://github.com/GauravAnand30/MedicalBot/blob/main/screen%20shot/Screenshot%202025-02-24%20004108.png)

## 📥 Installation

Follow these steps to set up and run the project:

### 1️⃣ Clone the Repository
```bash
git clone REPO_LINK
cd REPO_NAME
```

### 2️⃣ Create a Virtual Environment
```bash
python -m venv env
```

### 3️⃣ Activate the Virtual Environment
- **Windows:**
```bash
env\Scripts\activate
```
- **macOS/Linux:**
```bash
source env/bin/activate
```

### 4️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 5️⃣ Set Up Pinecone Database
1. **Create an account on Pinecone.**
2. **Set up an index** for storing embeddings.
3. **Add your Pinecone API key** to environment variables or a configuration file.

### 6️⃣ Run Index Storage Script
```bash
python store_index.py
```

### 7️⃣ Start the Application
```bash
python app.py
```

### 🎯 Access the Application
The application will be available at:  
👉 **http://localhost:8000/**

---

### 📌 Future Enhancements
- Integration with additional medical knowledge bases.
- Multi-agent system for better query resolution.
- Fine-tuned medical language models for improved response quality.

Feel free to contribute and enhance the **MedicalBot** project! 🚀

# Q&A Chatbot using Retrieval-Augmented Generation (RAG)

## 📌 Project Description

This project implements a **Q&A chatbot** based on **Retrieval-Augmented Generation (RAG)**. The RAG architecture combines information retrieval and text generation to enhance the chatbot's ability to provide accurate and contextually relevant answers. This chatbot retrieves relevant information from a knowledge base using embeddings, then generates answers with a **DeepSeek R1 model** via the **Groq API**. The entire system is implemented using the **LangChain framework** in Python, which provides the tools to build modular and scalable AI applications.

## 🚀 Tech Stack

This project uses the following technologies:

- **Python**: The primary programming language for the implementation (Recommended version: 3.8+).
- **LangChain**: A framework for building applications that use language models in a modular and scalable manner. It is used to implement the RAG architecture.
- **Ollama**: A service used to create **embeddings** (vector representations of text) that are essential for information retrieval.
- **DeepSeek R1 Model**: A generative model that produces natural language responses, used here for generating chatbot answers.
- **Groq API**: An API to access the **DeepSeek R1 model** for generating responses.


## 🛠 Installation & Setup

Follow these steps to set up the chatbot on your local machine:

### **1. Fork the Repository**

Go to the GitHub repository page and click on the "Fork" button in the top right corner. This will create a copy of the repository in your GitHub account.

### **2. Clone the Repository**

```bash
git clone https://github.com/nazmulhasan77/RAG_ChatBot.git
```

### **3. Create a Virtual Environment**

```bash
python -m venv myenv  # For Windows/Linux/Mac
source myenv/bin/activate  # Mac/Linux
myenv\Scripts\activate  # Windows
```

### **4. Install Dependencies**

```bash
pip install -r requirements.txt
```

### **5. Set Up Environment Variables**

Create a `.env` file in the root directory and add the following:

```ini
GROQ_API_KEY=your_groq_api_key
```

> **Note:** Never share your API key or commit it to GitHub.

### **6. Run the Chatbot**

```bash
streamlit run chatbot.py
```

## 📖 How It Works

1. **Indexing Phase:** The chatbot takes input from PDFs or other sources, splits the text into chunks, converts these chunks into embeddings using **Ollama**, and stores them in a **vector database**.
2. **Retrieval Phase:** The chatbot fetches relevant information from the vector database using **similarity search**. Retrieved information is then combined with the user’s query.
3. **Generation Phase:** The **DeepSeek R1 model** (via Groq API) generates a response.

## 🤝 Contributors

- **Md Nazmul Hasan**

---

**🚀 Happy Coding!**

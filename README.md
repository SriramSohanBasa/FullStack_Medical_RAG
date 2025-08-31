
# Full Stack Medical RAG Chatbot

This is a sophisticated, full-stack medical chatbot that leverages a Retrieval Augmented Generation (RAG) pipeline to answer medical questions based on a provided medical book. The chatbot is built with a powerful combination of technologies, including Flask, LangChain, Pinecone, and OpenAI, to provide accurate and context-aware responses.

## ✨ Features

- **Retrieval Augmented Generation (RAG):** The chatbot uses a RAG pipeline to retrieve relevant information from a medical book and generate human-like responses.
- **Vector Search:** The medical book is converted into vector embeddings and stored in a Pinecone vector store for efficient similarity search.
- **Hugging Face Embeddings:** The chatbot uses state-of-the-art sentence-transformer models from Hugging Face to generate high-quality embeddings.
- **OpenAI Language Models:** The chatbot uses OpenAI's powerful language models to generate fluent and coherent answers.
- **Web Interface:** The chatbot has a user-friendly web interface built with Flask and Bootstrap, allowing users to interact with it in a chat-like manner.
- **Scalable and Extensible:** The project is designed to be scalable and extensible, allowing you to easily add new knowledge sources or integrate with other services.

## 🚀 Technology Stack

- **Backend:** Flask, LangChain, Pinecone, OpenAI, Hugging Face
- **Frontend:** HTML, CSS, JavaScript, Bootstrap
- **Dependencies:** `sentence-transformers`, `langchain`, `flask`, `pypdf`, `python-dotenv`, `pinecone[grpc]`, `langchain-pinecone`, `langchain_community`, `langchain_openai`, `langchain_experimental`

## 📂 Project Structure

```
FullStack_Medical_RAG/
├── .gitignore
├── app.py
├── requirements.txt
├── store_index.py
├── template.py
├── Data/
│   └── Medical_book.pdf
├── research/
│   └── trials.ipynb
├── src/
│   ├── __init__.py
│   ├── helper.py
│   └── prompt.py
├── static/
│   └── style.css
└── templates/
    └── chat.html
```

- **`app.py`:** The main Flask application that handles the web interface and chat logic.
- **`store_index.py`:** A script to process the PDF, create embeddings, and store them in the Pinecone index.
- **`src/helper.py`:** Contains helper functions for loading the PDF, splitting text into chunks, and downloading Hugging Face embeddings.
- **`src/prompt.py`:** Defines the prompt template for the language model.
- **`templates/chat.html`:** The HTML template for the chat interface.
- **`static/style.css`:** The CSS file for styling the chat interface.
- **`Data/Medical_book.pdf`:** The medical book used as the knowledge source.
- **`requirements.txt`:** Lists the Python dependencies.
- **`template.py`:** A script to create the basic file structure of the project.
- **`research/trials.ipynb`:** A Jupyter notebook for research and experimentation.

## ⚙️ Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/FullStack_Medical_RAG.git
    ```

2.  **Create a virtual environment and activate it:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up your API keys:**

    Create a `.env` file in the root directory of the project and add your Pinecone and OpenAI API keys:

    ```
    PINECONE_API_KEY=YOUR_PINECONE_API_KEY
    OPENAI_API_KEY=YOUR_OPENAI_API_KEY
    ```

## 📖 Usage

1.  **Store the embeddings:**

    Run the `store_index.py` script to process the medical book and store the embeddings in your Pinecone index:

    ```bash
    python store_index.py
    ```

2.  **Run the Flask application:**

    ```bash
    python app.py
    ```

3.  **Open your browser and navigate to `http://127.0.0.1:8080` to start chatting with the medical chatbot.**

## 🙏 Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request if you have any suggestions or improvements.



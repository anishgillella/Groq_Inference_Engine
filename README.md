# Groq_Inference_Engine

# Chat Groq Demo

This repository contains a Streamlit application that demonstrates the usage of the ChatGroq model for answering questions based on provided context. The application integrates various LangChain components for document loading, text splitting, embeddings generation, and retrieval.

## Features

- Load documents from a web source.
- Split documents into manageable chunks.
- Generate embeddings using Ollama.
- Store embeddings in a FAISS vector store.
- Use ChatGroq model for generating responses.
- Retrieve contextually relevant documents and answer user queries.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/chat-groq-demo.git
    cd chat-groq-demo
    ```
2. Create a `.env` file in the root directory and add your GROQ API key:
    ```plaintext
    GROQ_API_KEY=your_groq_api_key
    ```

## Usage

1. Run the Streamlit application:
    ```bash
    streamlit run app.py
    ```

2. Open the application in your web browser:
    ```plaintext
    http://localhost:8501
    ```

3. Enter your prompt in the input field and get the response from the ChatGroq model. The application will also display the relevant document chunks used for generating the response.

## Code Overview

- `app.py`: The main file containing the Streamlit application logic.
- The application initializes various LangChain components, loads documents, splits them, generates embeddings, and sets up the retrieval chain.
- The user's input is processed, and the response along with relevant document chunks are displayed.

## Dependencies

- `streamlit`
- `langchain`
- `langchain_groq`
- `faiss-cpu`
- `python-dotenv`

Make sure to install all dependencies listed in the `requirements.txt` file.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements

- [LangChain](https://github.com/hwchase17/langchain)
- [ChatGroq](https://groq.com/)
- [Streamlit](https://streamlit.io/)

Feel free to contribute to this project by submitting issues or pull requests.

Here’s another version of your `README.md` for **Equity News Research Tool Using RAG**:

---

# **Equity News Research Tool Using RAG (Retrieval Augmented Generation)**

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/downloads/release/python-380/) [![Streamlit](https://img.shields.io/badge/streamlit-1.22.0-brightgreen)](https://docs.streamlit.io/) [![LangChain](https://img.shields.io/badge/langchain-0.0.284-blue)](https://python.langchain.com/en/latest/) [![OpenAI](https://img.shields.io/badge/OpenAI-API-brightgreen)](https://beta.openai.com/)

## **Introduction**

**Equity News Research Tool** is an AI-based web application that empowers users to extract insights from online news articles, focusing on equity markets and financial information. This tool utilizes **Retrieval Augmented Generation (RAG)** to combine the power of retrieval systems with advanced language models to provide informative and accurate responses to user queries about the processed news articles.

The goal is to make financial research easy, fast, and accurate by processing and indexing news articles, which are then used to answer specific questions from users. 

## **Features**
- **Multi-Article Processing**: Input up to 3 URLs for news articles and process them for analysis.
- **AI-Powered Question Answering**: Leverages OpenAI's language models and LangChain for answering questions about processed news articles.
- **Sources with Answers**: Provides context and references by showing the sources used to generate answers.
- **Embeddings and FAISS Indexing**: Efficiently indexes news content using embeddings and FAISS for quick retrieval.

## **Technology Stack**
- **Python** 3.8+
- **LangChain** `v0.0.284`
- **Streamlit** `v1.22.0`
- **OpenAI API** `v0.28.0`
- **FAISS-CPU** `v1.7.4`
- **Tiktoken** `v0.4.0`
- **Unstructured** `v0.9.2`

## **Getting Started**

### Prerequisites
- Python 3.8 or higher
- An OpenAI API key

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/equity-news-research-tool.git
    cd equity-news-research-tool
    ```

2. **Set up virtual environment**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # For Windows: venv\Scripts\activate
    ```

3. **Install the dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Configure environment variables**:
    - Create a `.env` file and add your OpenAI API key:
    ```bash
    OPENAI_API_KEY=your_openai_api_key
    ```

5. **Run the application**:
    ```bash
    streamlit run main.py
    ```

## **How to Use**

1. **Input URLs**: In the sidebar, input up to 3 URLs of news articles.
2. **Process the URLs**: Click the **Process URLs** button to load and analyze the articles. The tool will parse the content, split the text, and build embeddings for fast retrieval.
3. **Ask Questions**: Once the articles are processed, you can ask questions about the content. The AI will generate answers based on the indexed articles and display the sources.
4. **View Results**: The system will show the AI-generated answer along with the sources for further reading.

### Example

- **Input URLs**:  
  Enter news article URLs like _"https://news-site.com/article1"_.
  
- **Question**:  
  _"What are the latest trends in equity markets?"_

- **Answer**:  
  The tool provides an answer based on the content of the processed articles and lists the sources for reference.

## **Saving and Loading FAISS Index**

- **Saving**: The FAISS index containing document embeddings is saved as `faiss_store_openai.pkl` after processing.
- **Loading**: When a user asks a question, the application loads the FAISS index to perform fast retrieval and generate an answer.

## **Roadmap and Future Enhancements**
- **Additional File Support**: Extend the tool to accept more input formats, such as PDF documents or plain text.
- **Real-time News Fetching**: Add an option to pull live financial news from APIs and process them on the fly.
- **Improved User Interface**: Create a more intuitive interface with interactive visual elements to improve the user experience.
- **Multi-User Support**: Enable user authentication to allow multiple users to save and track their queries and research history.

## **Contributing**

We welcome contributions to improve this project. To get started:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add YourFeature'`).
4. Push to your branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## **License**

This project is licensed under the MIT License. See the `LICENSE` file for more information.

-

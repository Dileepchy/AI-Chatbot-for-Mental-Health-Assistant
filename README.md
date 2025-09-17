# Mental Health Chatbot 🧠💬

This project is a mental health chatbot designed to provide empathetic and informed support to users. It combines a powerful Large Language Model (LLM) with a dedicated sentiment classifier and a Retrieval-Augmented Generation (RAG) system to ensure responses are not only accurate but also emotionally resonant. 🤖❤️

-----

## **Key Features** ✨

  * **RAG-Powered LLM:** The chatbot uses a RAG framework to retrieve information from a curated knowledge base of mental health resources, providing evidence-based answers. 📚
  * **Sentiment Classifier:** A BERT-based model analyzes user input to determine their emotional state, allowing the chatbot to respond with an appropriate tone. 😔➡️😊
  * **Agentic Behavior:** The system can be configured to perform specific actions based on the user's needs, such as guiding them through a breathing exercise or providing a list of resources. 🧘‍♀️
  * **Semantic Search:** Utilizes semantic similarity to find the most contextually relevant information from the knowledge base. 🔎
  * **Interactive Interface:** A clean and user-friendly chat interface built with Streamlit. 💻

-----

## **Technologies Used** 🛠️

  * **LLM (Large Language Model):** The core of the chatbot. (e.g., GPT-3.5, LLaMA, or a fine-tuned open-source model). 🤖
  * **BERT:** Used for the sentiment analysis classifier due to its superior contextual understanding. 🧠
  * **RAG (Retrieval-Augmented Generation):** The architectural pattern for grounding the LLM with external knowledge. 🔗
  * **Streamlit:** The web framework used to create the user interface. ✨
  * **Python:** The primary programming language. 🐍
  * **Libraries:** Hugging Face `transformers`, `torch` or `tensorflow`, `faiss` or `chromadb` for vector search, `streamlit`. 📦

-----

## **Setup and Installation** 🚀

Follow these steps to get the project running on your local machine.

### **Prerequisites** ✅

  * **Python 3.8** or higher.
  * `git` installed on your machine.

### **Instructions** 📖

1.  **Clone the repository:**
    ```
    git clone https://github.com/your-username/mental-health-chatbot.git
    cd mental-health-chatbot
    ```
2.  **Create a virtual environment** (recommended):
    ```
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3.  **Install the required packages:**
    ```
    pip install -r requirements.txt
    ```
4.  **Download and set up the knowledge base:**
      * The RAG system requires a collection of mental health documents (PDFs, text files). Place these in a designated directory (e.g., `data/knowledge_base/`). 📂
      * Run the script to process the documents and create the vector store.
    <!-- end list -->
    ```
    python scripts/create_vector_db.py
    ```
5.  **Run the Streamlit application:**
    ```
    streamlit run app.py
    ```
    The application will open in your default web browser. 🎉

-----

## **Project Structure** 📂

  * `app.py`: The main Streamlit application file. 🚀
  * `sentiment_classifier/`: Contains the code and trained model for the BERT-based sentiment classifier. 🔬
  * `rag_system/`: Houses the RAG pipeline, including the vector store and retrieval logic. 🔄
  * `data/`:
      * `knowledge_base/`: Directory for raw mental health documents. 📝
      * `vector_store/`: Stores the processed vector database for RAG. 🗄️
  * `scripts/`: Utility scripts for data processing and model setup. ⚙️
  * `requirements.txt`: Lists all the necessary Python dependencies. 📜

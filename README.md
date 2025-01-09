
# TutorAI: Intelligent Document Retrieval and Question Answering System

TutorAI is a state-of-the-art AI-driven document retrieval and question-answering system that leverages OpenAI's GPT models, LangChain, and ChromaDB to provide intelligent insights from uploaded PDF documents. With advanced text chunking, embedding generation, and similarity-based retrieval mechanisms, TutorAI enables users to interact with their documents in an intuitive and efficient manner.

---

## 📜 **Table of Contents**

1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Setup Instructions](#setup-instructions)
5. [How It Works](#how-it-works)
6. [Usage](#usage)
7. [Visualization](#visualization)
8. [Future Enhancements](#future-enhancements)
9. [License](#license)

---

## 🌟 **Introduction**

TutorAI is designed to help users engage with their documents like never before. Upload academic papers, reports, or books, and TutorAI will split them into manageable chunks, embed them, and allow intelligent question-answering. By integrating advanced AI and ML techniques, TutorAI provides precise and contextually accurate answers while referencing the original document.

---

## 🚀 **Features**

- **PDF Upload and Parsing**: Load and process multiple PDFs seamlessly.
- **Text Chunking**: Splits large documents into manageable and context-rich chunks.
- **Embeddings with OpenAI**: Utilizes `text-embedding-3-small` for robust embedding generation.
- **Cosine Similarity**: Measures the similarity between document chunks for high-quality retrieval.
- **Document Visualization**: Visualizes embeddings in 2D using PCA for better understanding.
- **Multi-Query Retrieval**: Generates diverse question formulations to improve search accuracy.
- **Context-Based QA**: Answers questions strictly based on the provided document context, ensuring precision.

---

## 💻 **Technologies Used**

- **Python**: Core programming language.
- **LangChain**: Framework for building modular applications using LLMs.
- **OpenAI GPT Models**: `gpt-4o-mini` and `text-embedding-3-small`.
- **ChromaDB**: Vector database for efficient storage and retrieval of document embeddings.
- **Scikit-Learn**: PCA for dimensionality reduction and cosine similarity calculations.
- **Matplotlib**: For data visualization.

---

## 🛠 **Setup Instructions**

Follow these steps to set up and run the project on your local system:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/TutorAI.git
   cd TutorAI
   ```

2. **Install Dependencies**:
   Ensure Python 3.8+ is installed, then run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up OpenAI API Key**:
   Create a `.env` file in the project root and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key
   ```

4. **Load PDF Files**:
   Place your PDFs in the `TutorAI_Data/` directory.

5. **Run the Project**:
   Execute the script:
   ```bash
   python main.py
   ```

---

## 🔎 **How It Works**

1. **Document Loading**:
   - Loads all PDFs from the specified directory.
2. **Text Splitting**:
   - Uses LangChain's RecursiveCharacterTextSplitter to split text into chunks.
3. **Embedding Generation**:
   - Embeds chunks using OpenAI's `text-embedding-3-small`.
4. **Similarity Computation**:
   - Applies cosine similarity for efficient information retrieval.
5. **Query Handling**:
   - Processes user questions, formulates diverse variations, and retrieves the best-matching context.
6. **Answer Generation**:
   - Answers are generated strictly based on the retrieved context.

---

## 🧑‍💻 **Usage**

1. Upload PDFs to `TutorAI_Data/`.
2. Modify and run `chain.invoke()` to start querying your documents.
3. Visualize embeddings using the provided PCA functionality.
4. Retrieve answers with document references for traceability.

---

## 📊 **Visualization**

This project includes a visualization of document embeddings using PCA for a 2D projection. Below is an example scatter plot showing embeddings distributed across two principal components:

![Visualization Example](visualization.png)

---

## 🌟 **Future Enhancements**

- Add support for more file formats (e.g., DOCX, TXT).
- Enable real-time querying through a web-based interface.
- Expand multi-query retrieval with more robust LLM models.
- Implement user-friendly feedback loops for iterative improvements.


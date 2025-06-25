# 🧠 AI-Powered Course Search with OpenAI and Pinecone

This project builds a semantic search engine that lets users search through course data using natural language queries. It leverages **OpenAI embeddings** to capture the meaning of course descriptions and **Pinecone** as the vector database for fast and scalable similarity search.

---

## 📚 Project Description

The goal of this project is to enable **intelligent, meaningful search** across a dataset of tech-related courses. Traditional keyword search falls short when users search with abstract or fuzzy terms (e.g., "intro to web dev" or "AI for business"). By using vector embeddings and semantic search, this tool can return highly relevant course matches even when the query doesn’t directly match the text.

---

## ⚙️ Tech Stack

- **Python**
- **Pandas** – for data handling and preprocessing
- **OpenAI API** – for text embeddings
- **Pinecone** – for vector storage and semantic search
- **Tiktoken** – for tokenization (optional)
- **Dotenv** – to manage API keys securely

---

## 🧩 Project Structure

### 1. Import Libraries and Initialize Environment
Load all required libraries and set up environment variables for API access.

### 2. Load and Process Course Data
Read course data from a CSV file and generate structured metadata and formatted text descriptions.

### 3. Initialize Pinecone and Embeddings
Connect to Pinecone and configure the OpenAI embedding model.

### 4. Generate Document Texts and Embeddings
Embed course descriptions into numerical vector representations.

### 5. Create and Populate Pinecone Index
Create (or check for) a Pinecone index and batch upsert the vectorized course data with metadata.

### 6. Perform Semantic Search
Embed a query, perform similarity search in Pinecone, and display the top matching course results with their scores and descriptions.

---

## 🧪 Example Query

```python
query = "beginner course to learn front-end development"

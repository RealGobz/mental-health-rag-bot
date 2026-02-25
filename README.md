# Mental Health Semantic Assistant (RAG)

A lightweight Retrieval-Augmented Generation (RAG) bot that uses **GloVe Word Embeddings** for semantic search and **FLAN-T5** for natural language response generation.

## How it Works
Unlike traditional chatbots that use simple keyword matching, this assistant understands the **meaning** behind a user's question.

1.  **Vectorization**: Every question in the FAQ dataset is converted into a 50-dimensional vector using pre-trained GloVe embeddings.
2.  **Semantic Search**: When a user asks a question, we calculate the **Cosine Similarity** between the user's input and the database.
3.  **Augmented Generation**: The best-matching answer is retrieved and fed as "Context" into **Google's FLAN-T5** model to generate a conversational and empathetic response.



## Setup

1. **Clone the repo:**
   ```bash
   git clone [https://github.com/RealGobz/mental-health-rag-bot.git]

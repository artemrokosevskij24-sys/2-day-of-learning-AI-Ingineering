AI Engineering & Python Learning Journey 🚀

A complete log of my practical transition from basic Python programming and file handling to building AI applications using the Google Gemini API, vector embeddings, and local vector databases (ChromaDB).

📂 Repository Structure & Daily Progress

Day 1 — Python Fundamentals, Files & JSON

Hello.py — First introductory script stepping into programming.

variables.py — Working with data types, strings, and formatted text (f-strings).

condition.py — Conditional logic (if-elif-else) for decision making.

loops.py — Iterating through lists and working with structured data dictionaries.

students_file.py — Writing and reading raw text files (.txt).

json_practice.py — Structured data serialization and deserialization using Python's built-in json module.

Project Day 1.py — Mini-project combining loops, condition checks, status filtering, and JSON report generation.

Day 2 — Direct LLM API Integration

Stepping out of no-code tools and writing custom Python scripts to interact directly with large language models:

first_api_call.py — First direct connection to the Gemini API, ensuring secure key management via .env.

chat_with_gemini.py — Interactive text generation using user input (input()) and configured system instructions (system_instruction).

chat_with_gemini2.py — Multi-round dialogue loop (while True) maintaining chat history and context memory via chat.send_message().

Day 4 — Embeddings & Vector Search (ChromaDB)

first_embedding.py — Generating multi-dimensional vector embeddings using Gemini and computing semantic proximity manually via Cosine Similarity (numpy).

chroma_test.py — Setting up a local vector database (ChromaDB), configuring a custom Gemini embedding function, adding multi-topic documents, and executing vector search queries (collection.query()).

🧠 Key Learnings & Takeaways

Secure Secrets Management: Using python-dotenv and .env files to keep API keys safe and out of source control.

The google-genai SDK: Authenticating clients, generating text content, and embedding strings for semantic analysis.

Stateless vs. Stateful Chat: Understanding that LLMs are stateless by default; multi-round chat relies on libraries resending full conversation history behind the scenes.

Vector Representations: Converting natural language into numeric vectors to capture deep semantic meaning rather than relying on exact keyword matches.

Vector Databases: Leveraging ChromaDB for local vector storage, indexing, and fast similarity lookups.

🛠️ Tech Stack

Python 3.14

google-genai — Official Google SDK for Gemini models

chromadb — Local vector database for semantic search

numpy — Numerical computations for cosine similarity

python-dotenv — Environment variable loader

⚙️ How to Run

Install required dependencies:

pip install google-genai chromadb numpy python-dotenv


Create a .env file in the project root folder:

GEMINI_API_KEY="your_actual_api_key_here"


Run any script:

python chroma_test.py

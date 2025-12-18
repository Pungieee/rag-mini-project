# Financial Fraud Detection using Hybrid RAG

**CN230: Database Systems Mini-Project**  

This project was built for our CN230 Database Systems course. Our team of three wanted to explore whether LLMs could be improved at spotting financial fraud by combining two different types of databases: Vector and Graph.

---

## Purpose

Standard AI sometimes misses the "big picture" or specific connections in financial data.  
We built a Retrieval-Augmented Generation (RAG) system that uses:

- **Vector Database (FAISS):** Finds transactions that are similar to known fraud cases.  
- **Graph Database (Neo4j):** Maps relationships between accounts to track how money flows.

---

## Tech Stack

- **LLM:** Gemini 2.5-Flash  
- **Vector Database:** FAISS  
- **Graph Database:** Neo4j  
- **Framework:** LangChain  
- **Dataset:** [Synthetic Financial Datasets for Fraud Detection (Kaggle)](https://www.kaggle.com/datasets/ealaxi/paysim1)

---

## My Role

I was responsible for the core data pipeline and the retrieval setup:

- **Data Ingestion & Cleaning:** Processed the raw Kaggle CSV using Pandas, balanced fraud cases, and engineered features.  
- **Vector Implementation:** Set up the FAISS index and handled the embedding process using HuggingFace models.  
- **RAG & Graph Support:** Assisted in implementing RAG agents and Neo4j/Cypher logic to ensure Vector and Graph components communicated correctly.

---

## Key Learnings

- **Hybrid Retrieval:** Combining Vector and Graph data improved results; Graphs excel at connectivity questions while Vectors excel at similarity.  
- **Data Bottlenecks:** Handling 6M+ rows taught efficient sampling and memory management in Python.  
- **Prompt Engineering for Agents:** Learned to write prompts that guide the AI to use FAISS and Neo4j tools correctly.

---


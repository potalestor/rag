# RAG project

The RAG (Retrieval-Augmented Generation) project includes several key stages:

1. **Database Setup and Text Extraction**: First, you clone the project repository and set up the database (LanceDB). Then, the knowledge base is created by running the `markdown_to_text.py` script, which extracts text from the Hugging Face transformers library documentation.

2. **Reranker Implementation**: A reranker is integrated into the system to improve the relevance of retrieved documents. You experiment with enabling the reranker and adjusting parameters such as `top_k_retrieve` and `top_k_rank`. Performance comparisons are made by measuring response time and evaluating how the quality of retrieved context changes with and without the reranker.

3. **LLM Comparison**: The project also involves comparing the performance of different language models (LLMs), including one model from Nebius AI Studio API. Their outputs and answer quality are compared across several prompts.

4. **Evaluation Setup**: An evaluation dataset of 20 questions is created, and the "LLM as a Judge" approach is used to objectively assess the best configuration based on quantitative metrics.

The project deliverables include performance comparisons, a detailed analysis of the reranker and embedding models, and conclusions on how the system can be optimized for different scenarios.

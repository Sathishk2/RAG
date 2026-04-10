# RAG

Thanks for visiting my RAG Repository.

In this repository, I built RAG where I learn how to
1. Load and split the document into chunks
2. embed it into vector database
3. retrieve chunks based on the query

I have learnt how to do 
1. traditional RAG
2. multi-query retrieval (generate multiple variations of a question, retrieve document for each question, answers the main question)
3. RAG-Fusion (generate multiple variations of a question, retrieve document for each question, ranks documents: if documents appear in each question, its rank is higher, highest rank document is used as context, LLM generates final answer)
4. Query Decomposition (breaks a complex questions into 3 smaller sub-question, answers each sub-question, adds context relevant to the question, ONLY answers the LAST sub-question)
5. Query Decomposition (combines all answers from sub questions into final answer)
6. Step back RAG (reprhase a specific question into a more general one, retrieves context for both specific question and general questions)
7. HyDE-based RAG (Hypothetical Document Embeddings) (generate a scientific-style passage to answer the question, use this passage as document to answer question)
8. Logical Routing (uses an LLM to decide which documentation source (Python, JS, Go) should answer a user's question)
9. Semantic Routing (uses an LLM to decide how to answer a question (either as a physics or math expert) based on semantic similiarty)
10. Query structuring for metadata filters (turns natural language questions into structured, filterable search queries for a video database using an LLM)
11. Multi-vector retrieval (scrape webpages, summarize the documents, stores embeddings of both summaries and originals, after a question is asked it searches summaries and returns full documents)
12. RAPTOR (splits documents into small pieces, group similar chunks together using vector embeddings, summarize each cluster, then summarize summaries which forms a tree structure, queries can match fine-grained chunks (details) and higher-level summaries (concepts))
13. 

I use langflow and langchain to build RAG. 

Tutorial is from freecodecamp and Tech with Tim.

# LlamaIndex_Basics

Here is a consolidated list of the tasks i performed using LlamaIndex framework:

1. **Direct LLM Calls**: Learned to use the LlamaIndex LLM abstraction for direct API calls, covering simple Completion requests and stateful Chat sessions that manage message history.
2. **Data Ingestion & Indexing**: Used SimpleDirectoryReader to load raw documents into LlamaIndex Document objects. Built a VectorStoreIndex, the core component for RAG, to store vector embeddings of the data. Integrated with a persistent vector database (ChromaDB) for storing and retrieving vectors. Created a QueryEngine to execute queries against the custom knowledge base and retrieve relevant source documents to ground the LLM's answer.
3. **Advanced Querying & Multi-Source Data**: Implemented Natural Language to SQL conversion by connecting LlamaIndex to a structured data source (SQLite) via SQLAlchemy, allowing complex database queries with plain text prompts. Developed a RouterQueryEngine to intelligently route incoming user queries to the most relevant specialized query engine (e.g., send a question about one topic to a specific vector index, and a question about a different topic to another).
4. **Contextual Chat**: Utilized the ChatEngine with the condense_question chat mode to ensure the LLM maintains conversation history and context across multiple turns.

Agentic RAG (Retrieval-Augmented Generation)

There are two primary types of RAG workflows:

Traditional RAG – In this setup, a specific database or knowledge source is used. A user query is processed through a prompt and passed to an LLM (Large Language Model), which retrieves information from the predefined database and returns a response.

Agentic RAG – This approach introduces an intelligent agent that can dynamically decide which database or tool to use based on the context of the user’s query. Instead of being limited to a single source, the agent chooses the most relevant retriever or data source before generating the response.

In my project, I implemented two separate databases: one containing information related to LangChain and the other focused on Python. Depending on the user's question, the agent intelligently selects the appropriate retriever tool connected to the respective database and provides a relevant answer.

In the code, these retrievers are passed as tools to the agent, allowing it to route queries contextually and enhance the overall flexibility and accuracy of the RAG system.

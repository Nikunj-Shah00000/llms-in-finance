# How does Retrieval works in OpenAI? (Financial Analysis)

Retrieval in OpenAI is performed using the file_search tool when creating your assistant or a thread.
(It's declared in the same way as the code_interpreter tool, if you're familiar with it.)


## What does file_search tool do?
* File search tool is the **RAG** (**Retrieval Augmented Generation**) pipeline developed by OpenAI in their **Assistant AI** API.

* It enhances the Assistant's capabilities by incorporating external knowledge.

* When using this tool, OpenAI will process your documents: parse it, chunk it, create and store embedding in vector store, and then retrieve relevant chunks using both keyword and smeantic search.


## In this tools, OpenAI applies several built-in retrieval best practices to extarct efficently data from a document:
"
- Rewrites user queries to optimize them for search.
- Breaks down complex user queries into multiple searches it can run in parallel.
- Runs both keyword and semantic searches across both assistant and thread vector stores.
- Reranks search results to pick the most relevant ones before generating the final response.
"


## Vector Store:
OpenAI provides also a vector store creation when uploading files with a default chunking Stragey:
- max_chunk_size_tokens: 800 (can be customized)
- chunk_overlap_tokens: 400 (can be customized)
- It's using *text-embedding-3-large* model
- It returns 20 chunks (can be customized) with their relevancy score to the user query.

---

**Maintainer:** Nikunj Shah

Nikunj is a Software Developer passionate about exploring and applying AI technologies. He focuses on enhancing this project and welcomes contributions.

*   GitHub:
*   LinkedIn:
*   Email: nikunjshah0310@gmail.com

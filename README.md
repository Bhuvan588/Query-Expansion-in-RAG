# Optimizing RAG using Query Expansion :books: :robot:

Traditional or Naive RAG lacks in detailed context understanding and hence lacks in accurate data retrieval. This can be optimized by using the technique of query expansion using generated answers.

This demo utilizes Local Ollama model and ChromaDB along with Langchain

NOTE: The code is built on top of the code of this repo (Please refer this first )

## :gear: Working
![WhatsApp Image 2025-02-23 at 2 17 17 AM](https://github.com/user-attachments/assets/9368a243-1261-4ef7-b4b8-5298843a5c08)


[Image source](https://www.predli.com/post/rag-series-query-expansion)

The user query is first expanded using the LLM, and the refined query is used to retrieve relevant document chunks from ChromaDB. The retrieved context is then combined with the expanded query and passed to the LLM to generate the final answer

As we have expanded our query by the above, the new entity thus formed is called expanded query and hence the name Query Expansion.


## 	:computer: Installation

First are using Local model, we need to install [Ollama](https://ollama.com/).

Then clone this repository using 
```
git clone https://github.com/Bhuvan588/Query-Expansion-in-RAG.git
```

Then activate virtual environment in any repository using
```
python -m venv env
env\Scripts\activate
```

Now we need to download models from Ollama . Here I used 2 models - one for querying and another for embedding ( the choice is yours)

```
ollama pull llama3.2:1b
ollama pull nomic-embed-text
```

Now install dependencies using ``` pip install -r requirements.txt```

Add your pdf into this repo and rename as notes.pdf

Run the cells one by one to get answers to your desired questions!!










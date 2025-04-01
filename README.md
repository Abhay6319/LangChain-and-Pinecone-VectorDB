1. This is LangChain and Vector Database project which used to read documents and retrieve answers based on your Questions through ChatGPT API key.

2. Register into Pinecone and generate Pinecone API key and do the same with ChatGPT API key
  

4. We need to create .env file and put ChatGPT OpenAI key and Pinecone API key in it with the name already mentioned in the file 

5. Install all the Libraries required by :
pip install openai
pip install langchain
pip install pinecone
pip install pypdf

4.Download this code, the pdf file your choice or the file provide her in the Git and put all of them in a Folder and open that folder in VS code.

5. If this code isn't working :
vectors = embeddings.embed_query("How are you?")
vector_length = len(vectors)  

print("Vector length:", vector_length)


Then try this code

from langchain_pinecone import PineconeVectorStore
import pinecone
index = PineconeVectorStore.from_documents(
    documents=doc,
    embedding=embeddings,
    index_name=index_name
)

6. I have created a separate section because reading the pdf file generates a lot of metadata, so the metadata will be stored into separate file and it'll be created
automatically when we run the code

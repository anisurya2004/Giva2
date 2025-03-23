# Giva2

Steps to run the code locally - 
1. This is the second task of the Giva assignment. Download all files in the repo and save them locally.
2. Go to newsapi.org. Generate an API key to fetch the latest news. For evaluation purposes, I have written down the API key I used in '.env' file.
3. The dependencies are given in the requirements.txt. Use the following code to install all the dependencies - pip install fastapi pydantic faiss-cpu numpy sentence-transformers python-dotenv requests
4. Run main.py by executing the following line on terminal 'uvicorn main:app --host 0.0.0.0 --port 8000'
5. This will start the app on the local host (port number 8000).
6. The API endpoints are -
   GET '/' - Home. Prints that the API is running
   POST '/api/add_document' - Adds documents to the database from newsapi.org
   POST '/api/search' -  Give the query, top_k (number of similar documents required and defualt is 5), metric ('cosine' or 'dot': default is cosine)
7. I have tested this API using Thunderclient on vscode. Below are some screenshots of the same.

   

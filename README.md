MODULE 1 EXTRACTING THE DATA FROM THE SOURCE
Zepto Catalog Data Pipeline 
Description:     
This project implements a catalog-style data pipeline using books.toscrape.com as the public scraping-practice data source.     
The pipeline follows:
Scrape → Clean → Convert → Normalize → Store → Query → Analyze     
Data Source
Website: books.toscrape.com
The website is a public scraping-practice website and does not require login or an API key.   



MODULE 2 ANALYTICS OF TITANIC DATA AND MAKE THE PREDICTION ON IT           
Description:     
This module predicts whether a passenger survived the Titanic disaster using Machine Learning algorithms.
The Titanic dataset is analyzed, cleaned, preprocessed, and used to train different classification models.         
Titanic-Survival-Prediction/ │ ├── titanic.csv ├── Titanic_ML.ipynb ├── titanic_final_pipeline.pkl └── README.md                




MODULE 3 ZEPTO POLICY RAG SYSTEM               
Description:    
This project is a simple RAG (Retrieval-Augmented Generation) system that answers questions about Zepto policies.   
RAG pipeline     Documents >> Chunking >> Embeddings >> ChromaDB >> Query >> Intent Classification >> Retrieve Top 3 Chunks >> Generate Answer >> JSON Response      
Install the required libraries:  
pip install -r requirements.txt      
Run the FastAPI application:     
uvicorn main:app --reload          
Open:
http://127.0.0.1:8000/docs   
Build the Docker image:   
docker build -t zepto-rag .    
Run the container:     
docker run -p 7860:7860 zepto-rag    

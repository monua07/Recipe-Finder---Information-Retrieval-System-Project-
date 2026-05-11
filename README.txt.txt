##Hybrid Recipe Information Retrieval System

The system uses a hybrid retrieval approach:
BM25F (lexical search)
Dense Retrieval (semantic search)
RRF (fusion)
Top 5 results are used for evaluation



#Installation (Optional)

The notebook also installs required packages automatically in the first cell.

Or you can install the dependencies manually by running:

pip install -r requirements.txt



#project/
├── NC Final IR Project Code.ipynb
├── corpus_cleaned.csv
├── queries.csv
├── qrels.csv
├── qrels_pool_for_judging.csv
├── Food_Images/
├── run_hybrid.csv
├── metrics_summary.csv
├── requirements.txt



#How to Run the System:

1. Open Jupyter Notebook:
2. Open NC Final IR Project Code.ipynb
3. Run all cells in order


The notebook will: 
├── Install Dependencies 
├── Load Corpus and queries files for testing
├── Run Text Processing 
├── Add a Query Expansion for some common semantic terms
├── Build BM25F 
├── Build Dense Retrieval
├── Build Rank Reciprocal Fusion
├── Run a helper code for loading the Recipe Images
├── Build the Final Hybrid IR Search Model 
├── Run the 10 Test queries into the Hybrid Search Model 
├── Build the Test queries results (Top 5 results per query)
├── Upload and Run the Manual relevance judging file 
├── Evaluate the test results with P@5 and and nDCG@5
├── Build and export the Metrics Summary
├── In the very last cell: Allow user to run their own queries in the demo


#Running Queries:

1. In the notebook, Run the demo cell. 
2. Enter a query on recipe names, meal ingredients, cooking style, etc. where prompted: 

query = input("Enter your query: ")

*Example queries: - "Chicken and Rice" , "Easy ground beef dinner"

3. Press Enter after you finish typing


4. The system will return:

Top 5 ranked recipes
Scores
Ingredients and instructions
Images (if available)

5. To Run a new query, Run the demo cell and do the search process again


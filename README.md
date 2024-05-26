# Project Highlights
![atliq_tees](https://github.com/codebasics/langchain/assets/157373320/9bbf5928-58c8-40fb-b284-baab831a9604)
- AtliQ Tees is a t shirt store that sells Adidas, Nike, Van Heusen and Levi's t shirts
- Their inventory, sales and discounts data is stored in a MySQL database
- We will build an LLM based question and answer system that will use following,
   * Google Palm LLM
   * Hugging face embeddings
   * Streamlit for UI
   * Langchain framework
   * Chromadb as a vector store
   * Few shot learning
- In the UI, store manager will ask questions in a natural language and it will produce the answers

# Installation

1.Clone this repository to your local machine using:
```
  git clone https://github.com/patilabhi20/LLM_project
```
2.Navigate to the project directory:
```
  cd 4_sqldb_tshirts
```
3.Install the required dependencies using pip:
```
  pip install -r requirements.txt
```
4.Acquire an api key through makersuite.google.com and put it in .env file
```
  GOOGLE_API_KEY="your_api_key_here"
```
5.For database setup, run database/db_creation_atliq_t_shirts.sql in your MySQL workbench

# Usage
1,Run the Streamlit app by executing:
```
streamlit run main.py
```

2.The web app will open in your browser where you can ask questions

# Sample Questions
- How many total t shirts are left in total in stock?
- How many t-shirts do we have left for Nike in XS size and white color?
- How much is the total price of the inventory for all S-size t-shirts?
- How much sales amount will be generated if we sell all small size adidas shirts today after discounts?

# Project Structure
- main.py: The main Streamlit application script.
- langchain_helper.py: This has all the langchain code
- requirements.txt: A list of required Python packages for the project.
- few_shots.py: Contains few shot prompts
- .env: Configuration file for storing your Google API key.

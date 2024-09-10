
LangChain HR Analysis Project

Overview:
This project uses a combination of Pandas, SQLite, LangChain, and Hugging Face's Gemma 2B model to analyze HR data. 
The goal is to provide insights such as how many employees have a satisfaction level below 0.5, how many work in the sales department, 
and how many employees have left the company. The project integrates natural language processing (NLP) with database querying through 
LangChain's SQLDatabaseChain.

Project Structure:
langchain-hr-analysis/
│
├── HR_comma_sep.csv          # The dataset containing HR data
├── langchain_hr_analysis.ipynb  # Jupyter Notebook with the main code
├── requirements.txt          # List of dependencies to install
├── README.md                 # Project documentation
└── .env                      # (Optional) Environment file for API keys

Installation:

Step 1: Clone the repository
git clone https://github.com/JbaraGeorge/JbaraGeorge.git
cd langchain-hr-analysis

Step 2: Install the required dependencies
You can install the required dependencies using pip by running:
pip install -r requirements.txt

Step 3: Set up Hugging Face API Key
You will need a Hugging Face API key to interact with the Gemma 2B model. Create a .env file in the project directory and add your API token:
HUGGINGFACEHUB_API_TOKEN=your_hugging_face_api_token

Step 4: Run the Jupyter Notebook
To run the project, launch the Jupyter Notebook:
jupyter notebook
Open the langchain_hr_analysis.ipynb file in Jupyter and run the cells to perform the analysis.

Project Workflow:
1. Data Loading: The HR dataset (HR_comma_sep.csv) is loaded using Pandas.
2. Database Setup: The data is saved into an SQLite database (my_data.db).
3. LLM Integration: Hugging Face’s Gemma 2B model is used to convert natural language queries into SQL.
4. Database Querying: LangChain's SQLDatabaseChain is used to answer questions about the dataset.

Sample Queries:
- How many employees have a satisfaction level below 0.5?
- How many employees work in the sales department?
- How many employees have left the company?

Results:
Below are some sample queries and the results obtained:
- How many employees have a satisfaction level below 0.5?
  Result: 4583 employees
- How many employees work in the sales department?
  Result: 4140 employees
- How many employees left the company?
  Result: 3571 employees

Dependencies:
This project requires the following Python libraries, which can be installed via requirements.txt:
- pandas
- sqlite3
- langchain
- langchain-community
- langchain-experimental
- python-dotenv
- numpy


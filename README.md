# Web-Scraping-and-Text-Analysis-of-News-Articles Project

The purpose of this project is to perform web scraping and text analysis on a collection of news articles. The project involves retrieving textual data from specified URLs, conducting text analysis to extract insights, and computing various variables related to sentiment, complexity, and linguistic features of the articles. The goal is to gain practical skills in web scraping, text processing, and analysis, which are valuable in data science, natural language processing, and content analysis fields.

# Setup Instructions:

# Install Required Libraries:

Install the necessary libraries by running the following commands:
## pip install pandas beautifulsoup4 requests textblob textstat nltk

## Create Directories:

Create a directory named article_texts in the same location as your script. This is where the extracted article texts will be saved.
Prepare Input Data:

Create an Excel file named Input.xlsx containing at least two columns: URL_ID and URL. The URL_ID is a unique identifier for each article, and URL is the URL of the article you want to scrape.
Execution Steps:

## Web Scraping (Retrieving Article Texts):

The script starts by loading the input data from Input.xlsx.
It creates the article_texts directory if it doesn't exist.
For each row in the input data, it retrieves the URL and uses the requests library to get the HTML content of the page.
It then uses BeautifulSoup to parse the HTML and extract the article content within the <article> tag.
The extracted article content is saved in a text file named {URL_ID}.txt inside the article_texts directory.
Text Analysis:

The script then starts another loop to iterate through the input data.
For each article, it reads the previously extracted text from the corresponding text file.
It uses the TextBlob library to perform sentiment analysis, computing positive and negative scores, as well as polarity and subjectivity scores.
It uses the textstat library to calculate various text statistics, such as average sentence length, percentage of complex words, FOG index, etc.
The computed variables are collected for each article and stored in a list.
Output Data:

After analyzing all articles, the script creates a results list containing the computed variables for each article.
Saving Output:

The script creates a DataFrame from the results list, using the column names defined in output_columns.
The DataFrame is saved to an Excel file named Output_Data_Structure.xlsx.
Running the Script:

Place the script in a directory along with the Input.xlsx file.
Open a terminal or command prompt.
Navigate to the directory containing the script and input file.
Run the script using the command: python script_name.py (replace script_name.py with your script's filename).



## 1. Project Setup and Data Collection:

- Create a GitHub repository to store your project code and files.
- Set up the project structure, including folders for input data, output data, code scripts, etc.
- Download the input dataset from the provided link and save it as Input.xlsx.
- Choose a web scraping library (BeautifulSoup, Scrapy, Selenium, etc.) to extract article text from the URLs in the input dataset.
- Write a script to scrape the article content from each URL and save it as a text file with the appropriate name (URL_ID).

## 2. Text Analysis:

- Import the required Python libraries for text analysis and processing (NLTK, spaCy, etc.).
- Read the extracted text files from step 1.
- Perform text preprocessing: lowercasing, removing special characters, tokenization, stopword removal, etc.
- Compute the required text analysis variables based on the definitions provided in "Text Analysis.docx".
- Create functions for each variable calculation to maintain modularity.
- Store the computed variables in a suitable data structure.

## 3. Data Aggregation and Output:

- Create a DataFrame or a data structure to store the computed variables along with the original input data.
- Save the aggregated data as an Excel file named Output Data Structure.xlsx, following the provided structure.

## 4. Project Documentation:

- Write a README.md file in your GitHub repository to explain the project's purpose, setup instructions, and execution steps.
- Document the approach which has been considered for web scraping, text analysis, and variable computation.
- Include information about the tools and libraries used.
- Provide code examples and explanations for the main components of your project.

## 5. Presentation Preparation:

- Create a PowerPoint presentation containing the following sections:
    - Problem Statement
    - Tools Used
    - Approaches
    - EDA Insights (insights derived from the text analysis)
- Use visuals, graphs, and tables to effectively convey your findings.
- Keep the presentation concise and organized.

## 6. Project Evaluation:

- Make sure your code is modular and follows the PEP 8 coding standards.
- Ensure your code is well-documented with comments where necessary.
- Maintain the codebase on GitHub, making it public so others can review it.
- Include a proper README file in your GitHub repository.
- Follow the guidelines provided in the project description for evaluation metrics and live sessions.

## 7. Workflow and Execution:

- Provide a clear description of how to run your code in the README file.
- Include any command-line arguments or configuration files required for the project.
- Explain the step-by-step process of data collection, text analysis, and result presentation.

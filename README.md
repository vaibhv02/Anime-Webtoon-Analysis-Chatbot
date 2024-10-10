# Project Overview: Anime and Webtoon Content Analysis and Chatbot

This project involves building several tools to analyze webtoon content, perform sentiment analysis on user comments, and create a chatbot for interacting with content about "Castle Swimmer." Here’s a summary of the major tasks we’ve completed:

## Major Tasks

### 1. Content Classifier
- **Objective:** Create a basic content classifier for webtoon descriptions.
- **Tools Used:** Python, scikit-learn.
- **Steps:**
  - Created a small dataset of webtoon descriptions.
  - Preprocessed the data using `TfidfVectorizer`.
  - Implemented a Decision Tree Classifier to classify descriptions into categories such as Romance, Action, Fantasy, etc.
  - Evaluated the model's performance and adjusted parameters to improve accuracy.

### 2. Web Scraping
- **Objective:** Scrape content from web pages for analysis and chatbot training.
- **Tools Used:** BeautifulSoup, requests.
- **Steps:**
  - Sent HTTP GET requests to fetch webpage content.
  - Parsed the HTML content to extract relevant text (e.g., user comments, article body).
  - Stored extracted content in a structured format for further processing.

### 3. Sentiment Analysis
- **Objective:** Perform sentiment analysis on user comments.
- **Tools Used:** Python, TextBlob.
- **Steps:**
  - Scraped user comments from a specific webpage.
  - Applied TextBlob to analyze the polarity of comments.
  - Categorized comments into positive, negative, or neutral.
  - Summarized the results with percentages of positive vs. negative comments.

### 4. Chatbot Development
- **Objective:** Build a basic chatbot to answer questions about "Castle Swimmer."
- **Tools Used:** Python, NLTK (replaced with a custom tokenizer).
- **Steps:**
  - Scraped article content to use as the knowledge base for the chatbot.
  - Defined responses based on key phrases and keywords extracted from the content.
  - Implemented the chatbot using regular expressions for keyword matching.
  - Created an interactive loop to handle user queries and provide relevant responses.

### 5. Project Documentation
- **Objective:** Document the project setup and tasks.
- **Tools Used:** Markdown.
- **Steps:**
  - Created a `requirements.txt` file listing all necessary dependencies.
  - Summarized the major tasks and steps in this README.md file.

## How to Run the Project

1. **Set up the environment:**
   ```sh
   pip install -r requirements.txt

2. Run the content classifier:

   - Follow the steps in the Content Classifier section of the code.

3. Perform sentiment analysis:

   - Scrape the comments and run the sentiment analysis script.

4. Use the chatbot:

   - Run the chatbot script and interact with it using the predefined questions.

### Summary
This project demonstrates the integration of web scraping, content classification, sentiment analysis, and chatbot development using Python. Each task builds on the previous one to provide a comprehensive toolkit for analyzing and interacting with webtoon content.

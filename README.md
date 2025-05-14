# Sentiment Analysis on Internship Feedback

## Project Overview

This project performs sentiment analysis on internship feedback to evaluate the overall sentiment of the responses and uncover valuable insights that can help improve internship programs. By analyzing over 1,000 feedback entries, we classify the responses into positive, neutral, and negative sentiments using Natural Language Processing (NLP) techniques, specifically leveraging the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis model. 

### Objective

The main goal of this project is to:
- Evaluate the emotional tone of intern feedback to identify key strengths and areas for improvement in the internship experience.
- Provide actionable insights for program managers to refine internship structures and enhance the intern experience.

### Tools and Technologies Used
- **Python**: Core programming language for data analysis.
- **Pandas**: For data manipulation and analysis.
- **NLTK (Natural Language Toolkit)**: Used for text processing and sentiment analysis.
- **VADER (SentimentIntensityAnalyzer)**: A sentiment analysis tool to classify feedback sentiment.
- **Matplotlib**: For data visualization (e.g., sentiment distribution bar chart).
- **WordCloud**: To create visual representations of frequent words in feedback.
- **Excel**: For data export and analysis.

### Dataset

The dataset contains synthetic feedback from 1,100 internship participants. The feedback includes various types of responses ranging from positive, neutral, and negative sentiments to provide a real-world-like evaluation of internship experiences.

---

## Key Features

### 1. Data Preprocessing
- **Null and Duplicate Check**: Ensuring the dataset is clean by identifying and handling any missing or duplicated entries.
- **Feature Engineering**: Adding new features like word count and character count for each feedback entry.
  
### 2. Sentiment Analysis
- **VADER Sentiment Analysis**: Using the VADER sentiment analysis tool to classify feedback into three categories:
  - **Positive**: Feedback with a compound score greater than or equal to 0.05.
  - **Neutral**: Feedback with a compound score between -0.05 and 0.05.
  - **Negative**: Feedback with a compound score less than or equal to -0.05.

### 3. Data Visualization
- **Sentiment Distribution**: A bar chart visualizing the distribution of positive, neutral, and negative feedback.
- **WordCloud**: Word clouds for positive, neutral, and negative feedback to display the most common words in each sentiment category.
  
### 4. Theme-Based Sentiment Analysis
- **Themes**: Feedback is analyzed for specific themes such as Mentorship, Communication, Projects, Learning, and Support, and the average sentiment score is calculated for each theme.

### 5. Exporting Results
- **Excel Export**: The full sentiment analysis results are saved in an Excel file. Additionally, sentiment-specific sheets are generated to segregate positive, neutral, and negative feedback.

---

## Project Flow

1. **Data Loading**: The dataset is loaded into a Pandas DataFrame from an Excel file containing internship feedback.
2. **Exploratory Data Analysis**: Initial checks for missing values, duplicate entries, and basic statistics on the feedback.
3. **Sentiment Scoring**: Using VADER's compound score to assign a sentiment (Positive, Neutral, Negative) to each feedback entry.
4. **Data Visualization**:
   - A bar chart displaying sentiment distribution across the dataset.
   - Word clouds for each sentiment category to highlight the most frequent words.
5. **Theme-Based Analysis**: Identifying themes in the feedback (e.g., Mentorship, Communication) and calculating average sentiment scores for each theme.
6. **Exporting Results**: Saving the processed data and sentiment results in an Excel file with separate sheets for each sentiment type.

---

## Insights and Recommendations

### Final Insights:
- **Positive Feedback**: Over 50% of feedback responses were positive, indicating that the majority of interns had a good experience.
- **Negative Feedback**: Approximately 25–30% of feedback was negative, with issues related to mentorship, task clarity, and engagement.
- **Neutral Responses**: A notable portion of feedback fell into the neutral category, indicating room for improvement in intern engagement.

### Recommendations:
- **Strengthen Mentor Engagement**: Improve mentor-mentee interactions and regular check-ins.
- **Clarify Task Instructions**: Provide clearer instructions and expectations for tasks and projects.
- **Improve Onboarding**: Ensure the onboarding process is more interactive and engaging for new interns.
- **Regular Surveys**: Run periodic surveys to gather ongoing feedback and track intern sentiment over time.

---

## Files Included

- **sentiment_analysis.ipynb**: Python script that performs all the analysis, including data loading, sentiment classification, and visualization.
- **Internship_Feedback_Dataset.xlsx**: Sample feedback dataset.


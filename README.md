#  Google Play Store App Review Analysis (EDA Project)
This project focuses on exploratory data analysis (EDA), data wrangling, and visualization of the Google Play Store Apps dataset along with User Reviews data to uncover meaningful insights that can support data-driven business decisions.
# Table of Contents
- Project Description  
- Project Files Description  
- Dataset Contents  
- Variables Details of Dataset  
- Problem Statements  
- Technologies Used  
- Steps Involved  
- Key Insights  
- Conclusion  

# Project Description
This project performs an **Exploratory Data Analysis (EDA)** on Google Play Store applications and their user reviews to extract meaningful business insights. The analysis focuses on understanding **app characteristics, user preferences, ratings behavior, install patterns, and sentiment trends**.

By cleaning, transforming, and visualizing the data, the project identifies factors influencing app success such as **pricing model, content rating, category, app size, and update frequency**. The insights derived from this analysis can help **app developers, product managers, and marketers** make data-driven decisions to improve app visibility, user engagement, and overall performance on the Play Store.

# Project Files Description
This project consists of **one Google Colab notebook** and **two CSV datasets**.

# Executable File
- **Play Store App Review Analysis.ipynb**  
  Contains the complete EDA pipeline including data cleaning, transformation, visualization, and insights.

# Input Files
- **data set 1.csv (Play Store Apps Dataset)**  
  Contains detailed information about apps such as ratings, reviews, installs, pricing, size, and content rating.
- **data set2 - User Reviews.csv (User Reviews Dataset)**  
  Contains user reviews along with sentiment analysis scores.

# Output
All visualizations, tables, and insights are generated and visible directly in the Colab notebook.

# Dataset Contents
The project uses **two datasets scraped from the Google Play Store**, covering apps published between **2010 and 2018**.

**Apps Dataset** → App-level metadata  
**User Reviews Dataset** → User feedback and sentiment analysis  

Together, these datasets help analyze both **quantitative app performance metrics** and **qualitative user opinions**.
# Variables Details of Dataset

# Apps Dataset

| Variable | Description |

| App | Name of the application |
| Category | Category to which the app belongs (33 categories) |
| Rating | Average user rating (1–5) |
| Reviews | Number of user reviews |
| Size | App size (converted to MB) |
| Installs | Total number of installs |
| Type | Free or Paid |
| Price | Price of the app (USD) |
| Content Rating | Target age group |
| Genres | App genre(s) |
| Last Updated | Last update date |
| Current Ver | Current app version |
| Android Ver | Minimum Android version required |

# User Reviews Dataset

| Variable | Description |

| App | Name of the app |
| Translated Review | English translation of user review |
| Sentiment | Positive / Negative / Neutral |
| Sentiment_Polarity | Polarity score (-1 to 1) |
| Sentiment_Subjectivity | Subjectivity score (0 to 1) |

# Problem Statements

- Which categories have the highest number of apps?
- Are most apps free or paid?
- How important are ratings for app success?
- Which content rating category dominates the Play Store?
- Which categories receive the highest installs?
- How do installs and reviews relate to ratings?
- How does pricing affect ratings and installs?
- How does app size influence popularity?
- How frequently are apps updated?
- What is the distribution of user sentiments?
- Is sentiment polarity related to subjectivity?
- How do paid and free apps differ in sentiment trends?
- Does last update date impact app ratings?
  
# Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  

# Steps Involved

# 1️⃣ Data Cleaning
- Removed missing values from the **Rating** column  
- Filled null values using **mode/median** where appropriate  
- Removed duplicate app entries  
- Dropped invalid ratings greater than 5  

# 2️⃣ Data Transformation
- Converted **Reviews, Installs, Price, and Size** into numeric format  
- Removed special characters such as `+`, `,`, and `$`  
- Standardized app size into **MB**  
- Extracted additional features such as **log_installs** and **log_reviews**

# 3️⃣ Exploratory Data Analysis
- Conducted **univariate, bivariate, and multivariate analysis**
- Used visualizations to explore trends and relationships
- Created additional features like:
  - **Rating Group**
  - **Estimated Revenue**
  - 
# Key Insights

- Around **92% of apps are free**
- Nearly **82% of apps are rated “Everyone”**
- **Family and Game** categories dominate the Play Store
- **Communication apps** have the highest average installs
- Most apps have ratings between **3.8 and 4.5**
- Free apps receive significantly higher installs than paid apps
- **Facebook** has the highest number of reviews
- Larger apps (>90 MB) receive more reviews on average
- Sentiment analysis shows **positive reviews dominate**
- Paid apps generally have higher ratings but fewer installs
  
#  Conclusion

The analysis reveals that **free, family-friendly, and frequently updated apps** perform best on the Google Play Store. Developers aiming for higher installs should prioritize **free pricing models**, optimize **app size**, and ensure **regular updates**.

Paid apps can succeed if priced reasonably and kept lightweight. Categories such as **Events, Beauty, and Parenting** offer growth opportunities due to lower competition. Overall, **EDA helps minimize development risks** and enables **data-driven app strategy planning**.


✨ **Thank you for reviewing this project!**  

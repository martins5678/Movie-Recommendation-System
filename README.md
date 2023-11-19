[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://bankoleridwan.github.io/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bankoleridwan/)


## Introduction / Problem Statement
[![Banner](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/banner.jpg)](https://images.unsplash.com/photo-1485846234645-a62644f84728?auto=format&fit=crop&q=80&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&w=1459)


Company X, an online-based cinema, wants to improve its platform's user experience, engagement, and retention by providing a user-specific movie recommendation. We developed a movie recommender system using a content-based and collaborative filtering algorithm in this project. The result is an app that provides a user-specific recommendation similar to those used on leading platforms like Amazon, Facebook, and Netflix.


## Goal of the Project

> The goal is to build a movie recommendation app to make users' specific recommendations using content-based filtering, collaborative-based filtering, or hybrid.



## Skills and Tools Used
* Python
* Machine learning packages (Scikit-learn and nltk)
* Project Management: Trello Board
* Natural Language Processing (NLP)
* Data Cleaning
* Data Exploration
* Model Deployment: AWS EC2, S3 bucket and Streamlit
* Soft Skills: Presentation skill, Collaboration, Communication and Leadership


## Task Overview (My contribution)

Here is a concise high-level review of the critical tasks to achieve the project goal.
* Comprehensive data exploration to select features with a high correlation with movie ratings.
* Meticulous data cleaning procedures involve removing stop words and punctuation, tokenizing text, lemmatization, and vectorization.
* Calculated cosine similarity scores between users and movies and subsequently use it to predict user ratings for movies they had not watched content-based filtering.
* Built collaborative-based filtering models using surprise packages algorithm, including SVD, PMF, SVD++, and NMF
* Evaluated model performance using 1_score.


## Insights 
The data exploration reveals
* A wide variability in movies and users' ratings. While some users have rated 12,952 movies, others have just rated as few 1. Also, some moves have been rated 32,831, while others have just been rated once.
   * ### Top 20 MovieId Distribution
    ![top 20 movieId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Top%2020%20movieId.png)

   * ### Top 20 UserId Distribution
    ![top 20 userId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Top%2020%20userId.png)


* As shown above, the high variability can cause a cold start in collaborative filtering.
* To mitigate this challenge and enhance model performance, we filtered out users and movies with ratings below a threshold of 500.
* The Singular Value Decomposition (SVD) algorithm gave the best f1_score


## Outcome

Explore the user-friendly recommendation system app that makes user-specific predictions based on users' past three moves. 

### Recommender System App Demo

[![Recommender System App Demo](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/play%20icon.png)](https://www.youtube.com/watch?v=2VTIwhwER0A)


## Model Deployment

Subsequently, the app was deployed using an AWS EC2 instance and S3 bucket for widespread accessibility. 

## Acknowledgements

My Shout out goes to my team members for their contributions: 
* Toluwatise Onadipe
* Grace Quinn
* Kennedy Chege
* Chidinma Madukife



Ready to unlock the full potential of your data? I'm excited to collaborate and help your business thrive through data-driven insights. [Get in touch!](https://bankoleridwan.github.io/#contact:~:text=My%20Resume-,Contact%20Me,-Ready%20to%20unlock)


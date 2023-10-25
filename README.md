
# Movie Recommendation System

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://bankoleridwan.github.io/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bankoleridwan/)


## Introduction
[![Banner](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/banner.jpg)](https://images.unsplash.com/photo-1485846234645-a62644f84728?auto=format&fit=crop&q=80&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&w=1459)



The digital market is a promising space for any business that wants to thrive in this era. It makes a wide range of products, from content in entertainment to groceries and clothes, available at users' fingertips. With a plethora of choices available coupled with an average human attention span of 8.25 seconds, there is a solid need for a system to filter the available choices and narrow them down to products and services that the user is more likely to prefer.

The recommender system solves this challenge by providing personalized product and service suggestions based on users' historical data. In this project, we explored implementing a recommender system in the movie industry to provide personalized movie recommendations. We leveraged users' historical data and various movie information such as the cast, director, title and genres to deliver an unforgettable user experience that drives business growth.

There are three approaches to recommender systems: collaborative filtering, content-based filtering and hybrid. Collaborative filtering is based on historical data on users' interaction with the items to calculate user similarities and provide recommendations. Content-based filtering uses additional users or item information to find similarities between items and users and then provide a recommendation. Finally, a hybrid combines the principle of collaborative and content-based filtering.


## Goal of the Project

> To create a user-friendly movie recommendation system app that enhances users' experience, drives engagement, and fosters business growth by connecting users with content tailored to their interests, revolutionizing the movie-watching experience.

## Problem Statements

In today's technologically driven entertainment industry, users have many movie choices to make. As a result, coupled with a low human attention span, it is overwhelming to choose the right movie to watch, leading to a loss of user engagement and revenue for the entertainment industry. As a team of data scientists, we were tasked to design a user-friendly recommendation system using content-based and collaborative filtering to predict how a user will rate a yet-to-be-viewed movie based on their past preferences and then make movie recommendations based on the prediction. Solving this challenge offers economic potential by enhancing user experiences and generating revenue through tailored content recommendations.

## Outcome
We unearthed hidden patterns within the movie dataset using statistical analysis, programming, and machine learning techniques. Armed with this newfound knowledge, we trained a movie recommendation model to suggest films based on users' past preferences. Then, we designed an interactive and user-friendly dashboard using Streamlit to facilitate the practical utilization of the recommendation model. Finally, we deployed the model using an AWS EC2 instance and S3 bucket for global availability. 

## Skills and Tools Used
* Programming Language: Python
* Project Management: Trello Board
* Data Manipulation
* Unsupervised Machine Learning Algorithms
* Natural Language Processing (NLP)
* Data Cleaning
* Data Exploration 
* Model Deployment: AWS and Streamlit
* Soft Skills: Presentation skill, Collaboration, Communication and Leadership


## Data Preprocessing Issues
The provided dataset exhibited a high degree of normalization. It comprises various components, including genome scores, genome tags, an IMDb movie dataset, a movie dataset, a rating dataset, and a tags dataset. Our initial dataset assessment involved a meticulous examination to identify features of particular relevance.

In content-based filtering, we identified key factors that could significantly influence user movie preferences, such as genre, cast, director, plot keywords, and title. To harness the potential of these features, we merged the relevant separate data frames into a single data frame. We conducted data cleaning procedures involving removing stop words and punctuation, tokenizing text, lemmatization, and, ultimately, vectorization. Subsequently, we leveraged the results to calculate cosine similarity scores between users and movies. These user similarity scores were then employed to predict user ratings for movies they had not watched.

Furthermore, we developed a collaborative filtering-based model utilizing information about user_id, movie_id, and user ratings for each movie. For this task, we used the Surprise package, and among the various algorithms available, the Singular Value Decomposition (SVD) algorithm demonstrated superior performance, as evidenced by the F1_score metric.

One notable challenge encountered in collaborative filtering was the "cold-start" problem, which arises when making recommendations for new users or items. This issue was anticipated due to the dataset's broad user and movie rating distribution, from users who rated just one movie to those who rated up to 12,952 movies and movies with ratings ranging from 1 to as many as 32,831. To mitigate this challenge and enhance model performance, we implemented a filtering mechanism, excluding users with ratings below a threshold of 500 and movies with ratings below a similar threshold.

### MovieId Distribution Pattern

| Top 20 MovieId Distribution         | Last 20 MovieId Distribution        |
| ----------------------------------- | ----------------------------------- |
| ![top 20 movieId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Top%2020%20movieId.png) |  ![last 20 movieId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Last%2020%20movieId.png) |


### UserId Distribution Pattern

| Top 20 UserId Distribution          | Last 20 UserId Distribution         |
| ----------------------------------- | ----------------------------------- |
| ![top 20 userId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Top%2020%20userId.png) |  ![last 20 userId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Last%2020%20userId.png) |


## Model Building

Following the comprehensive data-cleaning process outlined previously, we built two distinct models. The first model adopts a content-based approach, harnessing natural language information from movie directors, casts, plot keywords, movie titles, and genres. This content-based model predicts user ratings for new movies they are yet to see, facilitating personalized recommendations.

Conversely, the second model takes a collaborative filtering approach, leveraging the Singular Value Decomposition (SVD) algorithm. 

In addition to model development and evaluation, we designed an interactive dashboard using Streamlit. This dashboard allows users to utilize our movie recommendation system interactively to enhance their movie selection process. It allows users to choose their preferred model, select the top three movies they wish the model to consider, and ultimately offers a streamlined interface for exploring movie recommendations.

The dashboard's capabilities and functionalities are demonstrated in the demo below. 

### The Recommender System App Interface

| The Recommender System App Homepage | Top 10 Recommendations              |
| ----------------------------------- | ----------------------------------- |
| ![Homepage](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Streamlit%20homepage.PNG) |  ![Recommendations](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Streamlit%20recommend.PNG) |


### Recommender System App Demo

[![Recommender System App Demo](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/play%20icon.png)](https://www.youtube.com/watch?v=2VTIwhwER0A)


## Model Deployment

Subsequently, we deployed the recommender system app on AWS using Aws EC2 instance and S3 bucket for public access. This deployment enables widespread accessibility, allowing users to benefit from its capabilities and personalized movie suggestions.



Ready to unlock the full potential of your data? I'm excited to collaborate and help your business thrive through data-driven insights. [Get in touch!](https://bankoleridwan.github.io/#contact:~:text=My%20Resume-,Contact%20Me,-Ready%20to%20unlock)

## Acknowledgements

My Shout out goes to my team members for their contributions: 
* Toluwatise Onadipe
* Grace Quinn
* Kennedy Chege
* Chidinma Madukife

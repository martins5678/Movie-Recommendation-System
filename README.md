
# Movie Recommendation System

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://bankoleridwan.github.io/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bankoleridwan/)


## Introduction
[![Banner](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/banner.jpg)](https://images.unsplash.com/photo-1485846234645-a62644f84728?auto=format&fit=crop&q=80&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&w=1459)



This project is centered on creating a dynamic movie recommendation system designed to deliver an unforgettable user experience and drive business growth. The objective is clear: to provide tailored movie suggestions based on user preferences and movie ratings. Leveraging collaborative filtering techniques, we aim to connect users with films that resonate with their tastes and interests.

This endeavor is driven by the collective vision of my team to enhance user engagement and satisfaction. In the subsequent sections, we will delve into the mechanics of collaborative filtering and its potential benefits for users and organizations. Together, we embark on a journey to revolutionize the movie-watching experience.

## Goal of the Project

> We aim to create an outstanding movie recommendation system that enhances user experiences and boosts our business. This project aims to enrich users' lives, drive engagement, and foster business growth by connecting users with content tailored to their interests, revolutionizing the movie-watching experience.

## Problem Statements

In our technology-driven world, recommender systems are pivotal for helping individuals choose content that aligns with their preferences. We seek to develop a recommendation algorithm, whether content-based or collaborative filtering, to predict how a user will rate a yet-to-be-viewed movie based on their past preferences and then make movie recommendations based on the prediction. Solving this challenge offers economic potential by enhancing user experiences and generating revenue through tailored content recommendations.

## Outcome
We unveil hidden patterns within the movie dataset using statistical analysis, programming, and machine learning techniques. Armed with this newfound knowledge, we trained a movie recommendation model to suggest films based on users' past preferences. Additionally, we developed an interactive and user-friendly dashboard using Streamlit to facilitate the practical utilization of our recommendation model.

## Skills and Tools Used
* Programming Language: Python
* Project Management: Trello Board
* Data Manipulation
* Machine Learning
* Natural Language Processing (NLP)
* Data Cleaning
* Data Exploartion 
* Model Deployment: AWS and Streamlit
* Soft Skills: Presentation skill, Collaboration, Communication and Leadership


## Data Preprocessing Issues
The provided dataset exhibits a high degree of normalization. It comprises various components, including genome scores, genome tags, an IMDb movie dataset, a movie dataset, a rating dataset, and a tags dataset. Our initial dataset assessment involved a meticulous examination to identify features of particular relevance.

In content-based filtering, we identified key factors that could significantly influence user movie preferences, such as genre, cast, director, plot keywords, and title. To harness the potential of these features, we aggregated them. We conducted data cleaning procedures involving removing stop words and punctuation, tokenizing text, transforming into root form using lemmatization, and, ultimately, vectorization. Subsequently, we leveraged the results to calculate cosine similarity scores between users and movies. These user similarity scores were then employed to predict user ratings for movies they had not watched.

Additionally, we developed a collaborative filtering-based model utilizing information about user_id, movie_id, and previous user ratings for each movie. For this task, we used the Surprise package, and among the various algorithms available, the Singular Value Decomposition (SVD) algorithm demonstrated superior performance, as evidenced by the F1_score metric.

One notable challenge encountered in collaborative filtering was the "cold-start" problem, which arises when making recommendations for new users or items. This issue was anticipated due to the dataset's broad user and movie rating distribution, from users who rated just one movie to those who rated up to 12,952 movies, and movies with ratings ranging from 1 to as many as 32,831. To mitigate this challenge and enhance model performance, we implemented a filtering mechanism, excluding users with ratings below a threshold of 500 and movies with ratings below a similar threshold.


| Top 20 MovieId Distribution         | Last 20 MovieId Distribution        |
| ----------------------------------- | ----------------------------------- |
| ![top 20 movieId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Top%2020%20movieId.png) |  ![last 20 movieId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Last%2020%20movieId.png) |



the wdqwdqwndqwdqwfefwddf
qwedwef
wef dqwefwe 


| Top 20 UserId Distribution          | Last 20 UserId Distribution         |
| ----------------------------------- | ----------------------------------- |
| ![top 20 userId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Top%2020%20userId.png) |  ![last 20 userId](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Last%2020%20userId.png) |


## Model Building

Following the comprehensive data-cleaning process outlined previously, we built two distinct models. The first model adopts a content-based approach, harnessing natural language information from movie directors, casts, plot keywords, movie titles, and genres. This content-based model predicts user ratings for new movies they are yet to see, facilitating personalized recommendations.

Conversely, the second model takes a collaborative filtering approach, leveraging the Surprise package. Among the various algorithms within this package, the Singular Value Decomposition (SVD) algorithm emerged as the top-performing choice. We trained the collaborative model using the SVD algorithm and evaluated its performance.

In addition to model development and evaluation, we designed an interactive dashboard using Streamlit. This dashboard empowers users to utilize our movie recommendation system to enhance their movie selection process. It allows users to choose their preferred model, select the top three movies they wish the model to consider, and ultimately offers a streamlined interface for exploring movie recommendations.

The dashboard's capabilities and functionalities are elaborated upon in the following section for a comprehensive overview of its features and user interaction possibilities.


| The Recommender System App Homepage | Top 10 Recommendations              |
| ----------------------------------- | ----------------------------------- |
| ![Homepage](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Streamlit%20homepage.PNG) |  ![Recommendations](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/Streamlit%20recommend.PNG) |


## Recommender System App Demo

[![Recommender System App Demo](https://raw.githubusercontent.com/bankoleridwan/Movie-Recommendation-System/main/img/play%20icon.png)](https://youtu.be/Vi4bUEh8I04)


## Model Deployment

Subsequently, we deployed our recommender system on the AWS EC2 compute services infrastructure, complemented by using an S3 bucket for public access. This deployment enables widespread accessibility to our movie recommendation system, allowing users to benefit from its capabilities and personalized movie suggestions.


Ready to unlock the full potential of your data? I'm excited to collaborate and help your business thrive through data-driven insights. [Get in touch!](https://bankoleridwan.github.io/#contact:~:text=My%20Resume-,Contact%20Me,-Ready%20to%20unlock)

## Acknowledgements

My Shout out goes to my team members for their contributions: 
* Toluwatise Onadipe
* Grace Quinn
* Kennedy Chege
* Chidinma Madukife

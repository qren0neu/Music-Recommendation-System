# Music-Recommendation-System

> This readme file is part of our final report.

## Introduction

This is the final project of INFO 6105 Data Science Methods and Tools

### About INFO 6105

Introduces the fundamental techniques for machine learning and data science engineering. Discusses a variety of machine learning algorithms, along with examples of their implementation, evaluation, and best practices. Lays the foundation of how learning models are derived from complex data pipelines, both algorithmically and practically. Topics include supervised learning (parametric/nonparametric algorithms, support vector machines, kernels, neural networks, deep learning) and unsupervised learning (clustering, dimensionality reduction, recommender systems). Based on numerous real-world case studies.

### Lecturer

Junwei, Huang

https://www.linkedin.com/in/junweih/

## Abstract

Recommendation systems are designed to help users discover new content they may like but have never consumed before. In this report, we introduce a new music recommendation system that employs multiple approaches to recommend music based on user input. We described the design of the system, including the methods used to recommend music and the metrics to evaluate the performance. We also conducted experiments using different parameter configurations, and compared the results with the existing music recommendation system.

## Background

Music recommendation is essential for music streaming services as it helps retain and attract customers. Personalized recommendations allow users to discover new music they enjoy, increasing their likelihood of continued use. In a crowded market, this differentiates a service and helps it stand out. Overall, music recommendation is valuable for music streaming services and for helping individuals discover new music.

## Project Summary

This project is aiming to build a content-based music recommendation system using a music genre dataset retrieved from Spotify. One simple idea is to recommend new music with the same genre tag as the one users listened to before. However, this approach might limit the diversity of the recommendations over time, as it narrows the range of selections.  
To overcome this drawback, we decided to build a recommendation system based on the acoustic characteristics, which might be similar across different genres of music. By considering a variety of acoustic features, our system will be able to provide personalized and diverse recommendations for users. 
In addition, we also created serval metrics to evaluate the effectiveness of the system, including the similarity between user input and our recommendations, the diversity of recommendations, and a comparison of our recommendations with those of Spotify.  

## Methodology

Here is a flow chart of how we designed the overall process.

![image](https://user-images.githubusercontent.com/110271091/217938882-8c274d0b-3746-42ee-ac4b-8ceefc9e069b.png)


## Experienments

Performance chart of using different clusters for recommendation:

<img alt="image" src="https://user-images.githubusercontent.com/110271091/217938120-0a437cc0-fcbe-41d7-b4d5-680f6a24b36b.png">

Performance chart of using different distance methods for recommendation

<img alt="image" src="https://user-images.githubusercontent.com/110271091/217938177-eb28cfeb-a58e-4ce8-883f-2ce1fdf935cc.png">

Performance chart of using different clusters and distance methods for recommendation

<img alt="image" src="https://user-images.githubusercontent.com/110271091/217938330-c9b623a0-3515-4e8f-a91c-7a8467d75a21.png">

Performance comparison between Spotify recommendations and our recommendations

<img alt="image" src="https://user-images.githubusercontent.com/110271091/217938387-a8f3b86c-928b-47d7-8390-5451ec69dc8d.png">

## Conclution and future works

In this report, we present a new music recommendation system that uses multiple approaches to suggest music to users based on their input. We provide details on the design of the system, including the techniques used for recommendation and the metrics used to evaluate its performance. We also conducted experiments with different parameter settings and compared the recommendations from our system and from Spotify.

Our recommendation system has several advantages. First, it can make recommendations for input music tracks that aren’t in our dataset. This was made possible because we created a function to obtain acoustic features of the input by using Spotify’s python library. Second, our comparison with the existing Spotify recommendation system has shown that our recommendations are diverse, and the similarity is close to Spotify's recommendations. Third, our recommendations are content based, so they are not restricted to a particular genre.

There are several ways to improve our system. One is to acquire more training data, which can be done by retrieving data from Spotify. Another is to look for additional evaluation metrics, such as user feedback. We can also explore other clustering algorithms such as DBSCAN and agglomerative clustering. Finally, we can adapt new mythology to enable more flexible adjustment of the existing algorithm. We can apply different weights to different steps, and new elements such as popularity and genre can be added. This will allow the algorithm to provide more personalized and accurate recommendations.

## Acknowledgements

The learning code is adapted from: https://www.kaggle.com/datasets/vicsuperman/prediction-of-music-genre and references therein. 

A few distance calculating and data processing algorithms are from: https://www.kaggle.com/code/vatsalmavani/music-recommendation-system-using-spotify-dataset/notebook

System, pipeline design & implementation: All by ourselves.

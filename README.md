# General info

This project was part of my thesis: 'Comparing collaborative filtering with content based filtering on Steam games', and marked my last project before graduating.
The main goal of the project was constructing both a collaborative and content based recommendersystem, to compare the performance of both of these techniques. 
In short, the project can be devided in the following tasks:
1. Cleaning the Steam user dataset
2. Cleaning the Games dataset
3. Creating a User-Item interaction matrix
	* This matrix represents all interacted items per user
4. Constructing the two recommendersystems 
	* Collaborative filtering / Content based filtering
5. Evaluating both models

## Collaborative Filtering

There are several ways to construct a collaborative filtering (CF) model, but the most conventional model is a Singular Value Decomposition(SVD) model. 
For this project, SVD was also used to construct the CF model.
SVD first decomposes the User-Item matrix, and then reconstructs it by calculating the dot product between the decomposed matrices. 
The 

## Content based Filtering

Content based filtering (CBF) focusses more on the contents of the items, in this case the games. 
It recommends games to users that are similar to the games the user already played, based on its contents. 
For this method the first step is to create user profiles for all users and item profiles for all items. 
After these profiles are built, they can be vectorized by a simple vectorizer. 
The last step is to calculate the similarities between the profiles based on the cosine similarity. 
The most similar items get recommended to the user. 

# Technologies

The project is coded in: Python V3.7

Using the following libraries:
* pandas
* numpy
* matplotlib
* seaborn
* scipy
* math
* random
* sklearn

Tools that were used:
Google colab
Anaconda
Overleaf / LaTeX
Mendeley

# Usage
The different models were tested and the results were noted in a seperate Excel file. After that the results were plotted in the CF model code file. 

# Note
This code was largely inspired by Gabriel Moreira, who made a recommender system for newspapers.
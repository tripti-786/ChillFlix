# ChillFlix - The Movie Recommender
A web application that suggests you movies of your choice. </br>
This project is a part of Microsoft Intern Engage 2022.</br>
Application can be accessed at: https://chillflix-the-recommender.herokuapp.com/ </br>
### Note:
The recommendation part developed by me in this web application doesn't support multi-language movies as it consumes 200% of RAM for generating Count Vectorizer matrix for all the 700,000+ movies in the TMDB. </br>
It only gives suggestions for hollywood movies.

## Introduction
This is a content based recommender system that suggest movies based on movie searched by the user. Also, it uses sentiment analysis to analyse the sentiments on the reviews given by the user. Apart from that, it shows the details of the searched movie, top casts and their details and user reviews for that particular movie.

## Tech Stack used
* HTML, CSS, JavaScript
* Python
* Flask
* Bootstrap
* API: TMDB (to fetch title, genre, rating, runtime, overview, poster etc., of the movie using the IMDB Id of the movie in the API)
* Deployed on Heroku
 

 ## Sources of Datasets
* [IMDB 5000 Movies Dataset](https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset)
* [The Movies Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset) --> please download credits.csv and movies_metadata.csv only
* [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
* [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
* [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)
#### Note:
I have not attached credits.csv file as that file is of large size and Github doesn't allow to upload such large files. Please download [credits.csv](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset?select=credits.csv) separately and paste it to the project folder/directory.

## How to run the project
* You will need to have [Python 3](https://www.python.org/downloads/) installed on your system.
* Clone/Download the repository to your local machine.
* Install the dependencies via command ```pip install -r requirements.txt``` --> in case if you get any error while installing dependencies then try to install dependencies one by one via command ```pip install library_name```
* Open the terminal/command prompt from your project directory and run the file main.py by executing the command ```python main.py```
* On the terminal you can see the localhost link. Click on that link by ```ctrl+click``` or type manually ```http://127.0.0.1:5000 ``` on your browser.
* Enjoy the project.

## Similarity Score
To decide which movie is similar to the movie that user likes; Cosine Similarity has been used. </br>
Cosine Similarity is a matrix used to measure the similarity of two vectors. Specifically, it measures the similarity in the direction or orientation of the vectors ignoring differences in the magnitude or scale.</br>
Both vectors need to be part of the same inner product space, meaning they must produce a scaler product through inner multiplication. </br>
The similarity of two vectors is measured by the cosine of the angle between them.
![cosine similarity](https://user-images.githubusercontent.com/92995593/170736683-80ef346e-7b08-4be7-8633-0e68a96b5db4.png)

## Flowchart
![flowchart](https://user-images.githubusercontent.com/92995593/170861295-cd6cc20d-fa5a-4474-b6f0-cdd598a3b470.png)


## Project home page
![Screenshot (179)](https://user-images.githubusercontent.com/92995593/170736780-5b732991-3339-4b6c-8d40-055e0fc3b995.png)


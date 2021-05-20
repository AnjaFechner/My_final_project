# Book into movie prediction - Gives the New York Times bestseller list for books (fiction/non-fiction) a hint for books that could be a movie in the future?
## Final Bootcamp Project
*Anja Fechner*

### Mai 2021*
***
![titel_bild](https://github.com/AnjaFechner/My_final_project/tree/main/pictures/titel_bild.png)

Project collecting, exploring, evaluate and visualize the data and make a predict with the dataset by using the Random Forest model. After that 


## Content
***

- [Introduction](#introduction)
- [The Data](#the-data)
- [Visualisation](#visualisation)
- [Statistical Analysis](#statistical-analysis)
- [Review](#review)
- [OnePager](#onepager)
- [Presentation](#presentation)

## Introduction
***

The influencer Lucy writes about books. At the moment she writes about books of her favourite authors and she takes into account the recommendations of friends and follower. 
Now, she wants to add a new category to the own channel. She wants to write about books that will be made into films. There are a lot of books and the following graph illustrated that about 2.110 books/short stories are the base for films during the years 1995 to 2020. 
That are around 81 books per year. She ask us, a media agency, for help. She needs a model to help her identify books that will be made into films.
But the model should be easy to use and of course, the data should ideally be available free of charge.

![books_movies_NA](https://github.com/AnjaFechner/My_final_project/tree/main/pictures/books_movies_NA.PNG)


## The Data 
***

We collected the data from freely available sources, like Wikipedia, Kaggle, etc. With this, we created a dataset of about 580 1st place books. 
The books were all in the first place on the New York Times bestseller list (genre: fiction and non-fiction). The data set contains 65 books that are made into a film.
Now, with this data set and the chosen free available information about the books (price, rating, review).

I used Python, Tableau and Excel to create the data set and applied the Random Forest and as an improving option the Logistic Regression and next to that the Random Forest model again.


## Visualisation
***

The graphs for exploring and evaluate the data set are published behind the link: [Link](https://public.tableau.com/profile/anja.fechner#!/).
The Tableau [file](https://github.com/AnjaFechner/My_final_project/tree/main/Tableau) is saved in the Repo, too.

## Statistical Analysis 
***

We explore the data set that is marked by the huge imbalance between the books and books that are made into a film.
The data set consists of only 3 free available features to analyze what determining factors why a book is predicted to make into a film.
Our target variable is the book adaption ('Yes'/'No').
We try to predict our target variable with the Random Forest model and as an improving option the Logistic Regression with the Random Forest.
But the huge imbalance in the data set and the low amount of features prevents the best solution. 


Overview of books (color: orange) and book adaptions (color: brown):
![Step_1](https://github.com/AnjaFechner/My_final_project/pictures/Step_1.PNG)

Some interesting features:
For a practical use, we take 3 books from the New York Bestseller list of 2021 and show what our model calculated.

The 3 books with the 3 features:
![test_books](https://github.com/AnjaFechner/My_final_project/tree/main/pictures/test_books.PNG)

The result of the model:
![test_result](https://github.com/AnjaFechner/My_final_project/tree/main/pictures/test_result.PNG)

The jupyter notebook files:
*Please note that the csv-xlsx files are linked to the jupyter notebooks*

The files are divided into 8 different steps.

- [Step 1](https://github.com/AnjaFechner/My_final_project/main/Step_1_web_scraping_nyt_bestseller/Step_1_Scraping_New_York_Times_Bestseller_Books_wikipedia.ipynb) 
Step 1 includes the web scraping of the bestseller list of books (genre fiction/non-fiction).

- [Step 2](https://github.com/AnjaFechner/My_final_project/main/Step_2_data_wrangeling/Step_2_Data_Wrangeling.ipynb)
Step 2 shows the first data wrangling steps on the data set.

- [Step 3](https://github.com/AnjaFechner/My_final_project/main/Step_3_web_scraping_AMZ_error/Step_3_Web_Scraping_AMZ.ipynb)
Step 3 shows the web scrapiing of the additional inforamtions for the books. This step failed.

- [Step 4](https://github.com/AnjaFechner/My_final_project/main/Step_4_join_the_files_bs_books_and_rating/Step_4_join_files-books_and_ratings_for_books.ipynb)
Step 4 shows the first joining of the dataset books and the data set with the additional features from different files and sources.

- [Step 5](https://github.com/AnjaFechner/My_final_project/main/Step_5_book_into_films/Step_5_Web_Scraping_book_into_movie.ipynb)
Step 5 includes the web scraping of book titles that were filmed.

- [Step 6](https://github.com/AnjaFechner/My_final_project/main/Step_6_join_bestseller_books_with_films/Step_6_Join_bestseller_books_with_films.ipynb)
Step 6 is the joining of the book list with features and the book adaptions list.

- [Step 7](https://github.com/AnjaFechner/My_final_project/main/Step_7_apply_NLP_and_Random_Forest/Step_7_NLP_and_Random_Forest.ipynb)
During Step 7 the Random Forest model will apply first time.

- [Step 8](https://github.com/AnjaFechner/My_final_project/main/Step_8_try_to_improve_the_model/Step_8_try_to_improve_the_model.ipynb)
Step 8 includes options to improve the model.


## Review
***

After the applicationof the models and discuss the results it is important to consider more features and to handle the imbalance of the data set with SMOTE. 
The search criteria werethe book title because we scraped the bestseller list starts with the year 1931 and this books has no ISBN. Through the various project steps, they have resulted in changes and this allows now to use the ISBN as search criteria. 
Now, the ISBN as search criteria is very important, because there are lots of variants in the book titles that the ISBN is the definitely best search criteria.


## OnePager
***

The OnePager is located in this [folder](https://github.com/AnjaFechner/My_final_project/main/one_pager).


## Presentation
***

The presentation is located in this [folder](https://github.com/AnjaFechner/My_final_project/main/presentation).
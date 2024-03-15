![image](https://github.com/varshil009/NetflixClustering/assets/118505855/a1f8976c-f631-487d-b89c-701df543f840)


# NetflixClustering
Using netflix dataset, making a recommender system using unsupervised learning models. The dataset have 7787 rows.

# Output pics
![WhatsApp Image 2024-03-15 at 4 12 19 PM](https://github.com/varshil009/NetflixClustering/assets/118505855/344fe647-80a4-474c-894a-bcd27667cd8a)

# Data Scrapping
In this dataset there were many missing values in cast and director features, I filled those values using **Selenium** webdriver. The process goes like this...
<ol>
<li>Program opens imdb site in a chrome tab</li>
<li>finds search box fills the value, finds search button clicks it</li>
<li>imdb site leads to search result, finds appropriate title (In cases of same titles) and clicks on it</li>
<li>Upon coming on title content page, It finds the element where cast or director text is visible, extracts text from it and fills directly to dataframe</li>
Although it can fill the value automatically the process takes too much time, because instead of scrapping directy we have to search and identify the particular content to fill those values. My experience says that to fill 200 values it might take 1.5 hours.
</ol>
<br>

# IMDbPY
### The scrapping using webdriver turned out to be time consuming and error prone to dynamism of modern websites. Although I wrote the program to bypass the pop-ups and hidden links, it is still time consuming. 
### I'm using this module instead, it connects to imdb data and fetches the relevant information. ( BTW This too took around 5 hours to only fill the missing 2000 rows of data.)

Also follow the imdb guidelines for using bots to extract and using data their data.
![Can I use IMDb data in my software?](https://help.imdb.com/article/imdb/general-information/can-i-use-imdb-data-in-my-software/G5JTRESSHJBBHTGX?ref_=helpart_nav_18#)

# Modules / functions / algorithms used...
[![Pandas](https://img.shields.io/badge/-Pandas-yellow?style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/-NumPy-blue?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org/)
[![scikit-learn](https://img.shields.io/badge/-scikit_learn-orange?style=flat-square&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/)
[![NLTK](https://img.shields.io/badge/-NLTK-green?style=flat-square&logo=nltk&logoColor=white)](https://www.nltk.org/)
[![pickle](https://img.shields.io/badge/-Pickle-lightgrey?style=flat-square&logo=pickle&logoColor=white)](https://docs.python.org/3/library/pickle.html)

<br>

[![KNN](https://img.shields.io/badge/-KNN-yellowgreen?style=flat-square)](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)
[![Nearest Neighbours](https://img.shields.io/badge/-Nearest_Neighbours-yellowgreen?style=flat-square)](https://en.wikipedia.org/wiki/Nearest_neighbour_algorithm)
[![PCA](https://img.shields.io/badge/-PCA-purple?style=flat-square)](https://en.wikipedia.org/wiki/Principal_component_analysis)
[![Silhouette Score](https://img.shields.io/badge/-Silhouette_Score-blueviolet?style=flat-square)](https://en.wikipedia.org/wiki/Silhouette_(clustering))
[![Cosine Similarity](https://img.shields.io/badge/-Cosine_Similarity-lightgrey?style=flat-square)](https://en.wikipedia.org/wiki/Cosine_similarity)


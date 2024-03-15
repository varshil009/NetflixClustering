![image](https://github.com/varshil009/NetflixClustering/assets/118505855/a1f8976c-f631-487d-b89c-701df543f840)


# NetflixClustering
Using netflix dataset, making a recommender system using unsupervised learning models. The dataset have 7787 rows.

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

## Modules / functions / algorithms used...
<a href="https://pandas.pydata.org/" target="_blank"><button>Pandas</button></a>
<a href="https://numpy.org/" target="_blank"><button>NumPy</button></a>
<a href="https://scikit-learn.org/stable/" target="_blank"><button>Scikit-Learn</button></a>
<a href="https://scikit-learn.org/stable/modules/neighbors.html" target="_blank"><button>KNN</button></a>
<a href="https://scikit-learn.org/stable/modules/neighbors.html" target="_blank"><button>Nearest Neighbors</button></a>
<a href="https://www.nltk.org/" target="_blank"><button>NLTK</button></a>
<a href="https://docs.python.org/3/library/pickle.html" target="_blank"><button>Pickle</button></a>
<a href="https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html" target="_blank"><button>PCA</button></a>
<a href="https://scikit-learn.org/stable/modules/generated/sklearn.metrics.silhouette_score.html" target="_blank"><button>Silhouette Score</button></a>

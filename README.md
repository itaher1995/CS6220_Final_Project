# CS6220_Final_Project

Paper Deliverable

**1. Abstract** <br />
Music is often divided into genres as a way to aggregate similar music and themes. However, in reality what we often find is musicians interact with musicians from different genres and create songs which have aspects of more than one genre. As a result, there is a case for exploring how genre identification performance varies between unsupervised and supervised machine learning models. This project attempts to explore those differences by approaching this problem through classification (SVM) and clustering (GMM). These algorithms will be applied to Free Music Archive dataset and features created from text mining of the corresponding lyrics. Via our classification algorithm we will attempt to classify the dataset into the 16 genres identified in the dataset. We will then compare the results of our classification to clustering to see how the dataset is grouped from an unsupervised perspective.  
<br />
**2. Introduction**<br />
Music has intrinsic properties that cause individuals to either like or dislike a set of given songs. These properties are used to aggregate similar songs into genres. It is commonly understood that users of music sharing/listening platforms, such as Spotify, create playlists based on genre. However, these users may create playlists based on mood or certain activities, such as working out or social events at bars or clubs and these playlists consist of songs that illicit similar reactions from the listener. While many of these playlists will consist of songs from the same genre, it is also possible that these playlists will have similar songs from different genres; causing us to ask the question of whether grouping songs by genre is the correct method for dividing music. The goal of this paper is to see how classification, in this case the various kernels of Support Vector Machines, of music performs compared to clustering of songs, for which we will use Gaussian Mixture Models.
 <br /><br /> The use cases for our findings mainly devolve into playlist creation. Based on what conclude is the correct methodology for aggregating songs, users can then create playlists based on similar songs within a song or classification. For example, if the classification model(s) identify genres very well we can state that given our predictors, a design matrix, _X_, we can correctly identify prelabeled classes, _Y_, and there is no need to update our current method of using genres. However, if the performance metrics indicate that the classification models can't associate predictors with their correct classes and the intra-cluster variance is low for clustering, then it can be said that the baseline of aggregation of songs, genres, is either outdated or simply incorrect and new categorizations may be needed for songs to properly bucket similar music.
<br /><br />
**3. Related Work** <br />
Previous iterations of music classification have been attempted using solely supervised machine learning. For example, Li Guo et. al. used the same dataset used in this project and developed classification models in an attempt to classify the dataset. The paper uses several multi-class classification algorithms, including Neural Networks, Softmax Regression and Support Vector Machines. They found that the Support Vector Machine with the Radial Basis Function provided the best performance on their test set.
<br /> <br />

**4. Methodology** <br />
The dataset used is a collection of songs from the [Free Music Archive](https://github.com/mdeff/fma). It is a collection of a few different files which include metadata regarding the tracks, features extracted using a library called [LibROSA](librosa.github.io/librosa/) for Python. Also, file that contains features from echohonest (now Spotify) was provided in FMA dataset. The dataset has in total 780 variables. The features extracted using LibROSA are representative features of the original audiofiles and have been aggregated into different representative statistics for each song (e.g. kurtosis.)

The preprocessing for this dataset included removing features that were largely unavailable in our dataset. The reason these features were not available is because the FMA archive contains songs that are from independent artists so certain variables, such as the rank of the artist or song were unavailable because they were never calculated.

Visualizing the distributions using qq-plots exposed the non-normality of many variables in the dataset. In order to make the distributions of each variable Gaussian-like, first we normalized the data to be between [0,1] and then various box-cox transformations were applied to the variables based on the following skew measurement, Pearson's second coefficient for skewedness. <br /><br />
* **Data Collection** <br />

* **Data Preprocessing** <br />

* **Dimensionality Reduction Techniques** <br />

* **Baseline Models** <br />

* Other Models

5 .Discussion

* **Discuss Baseline**

* Discuss Other

6. Conclusion

* Derive insight, is 16 genres the best way to classify genres

7. Future Work

# Movie Plot Synopsis Tagging

![](image.jpg)

In this case study, we will tag a movie based on the plot synopsis with 71 tags set. In general, movies are tagged with 3 or 4 tags, so, we also made models with 3 or 4 tags.


## Dataset

- Dataset used was MPST-2018 dataset. Please find the paper here: https://www.aclweb.org/anthology/L18-1274

Contains all the IMDB id, title, plot synopsis, tags for the movies. There are 14,828 movies' data in total. The split column indicates where the data instance resides in the Train/Dev/Test split.


## Real world Objectives and Constraints

 - Predict as many tags as possible with high precision and recall.
 - Incorrect tags could impact movie search results generated based on tags.
 - No strict latency constraints.

## Tagset

 - Contains 71 tags.
 ![](tags.png)
 
## Results:

The best performance is shown by LogisticRegression with all w2v, bow and tfidf features together giving <b>0.4101</b> f1-micro.

The performance of Top3 Tags LR model is <b>0.6102</b> f1-micro.

The performance of Top4 Tags LR model is <b>0.5874</b> f1-micro.

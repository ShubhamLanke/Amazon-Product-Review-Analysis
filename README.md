# Amazon-Product-Review-Analysis

1. Load the “Health and Sports” dataset which we downloaded from
    http://jmcauley.ucsd.edu/data/amazon/ i.e. amazon review dataset.
2. Initially the analysis will be done separately for both the categories
    Health and Sports.
3. Now import the data in Jupyter notebook, the total length of data will
    be about 6 lakh review data.
4. Later we will check for any null values if they are there in data set
    and later will group the data based on their ratings.
5. To reduce the workload on the system and processing time we will
    randomly sampling the data to 25000.
6. Later it will generate the pie chart based on the rating of the
    products.
7. The next function will remove any unnecessary spaces in text and
    will clean all numerical data.
8. Now we are removing all the stopwords using spacy library. The
    stopwords wont any value to the analysis, since it doesn’t have any
    semantic weightage
9. Followed by this is the lemmatization process to get the root word
    (with useful meaning). The lemmatization is done using the nltk
    lemmatizer.
10. Using this dataset, we’ll create the Vader and Bert model to analyse
    the sentiment of the given review dataset.
11. The Bert model is created using the pipeline. we are
    using multilingual model to get the output
12. The multilingual model gives output in the form of labels, higher the
    stars the more positive the sentence is.
13. The number rightly predicted data is high for the Bert model than the
    Vader model
14. The Vader model has good prediction for excellent category but has
    very bad prediction for other categories. Hence, we can use the
    output from the Bert model for further analysis.
15. Using this you can see the difference between Vader and neural
    network model. The sentiment of the sentence is predicted very well.
16. Now taking only the products having high number of negative
    sentiments. Understanding which words contributed to negativity of
    the sentence using “word cloud”.
17. Now we are finding the name of the product using named entity
    recognition. Where the some of the above predicted product’s name
    can be said as the product but not all the products is predicted very
    well.
18. Hence, we can use topic modelling to find out what the text is about
    and try to get the products
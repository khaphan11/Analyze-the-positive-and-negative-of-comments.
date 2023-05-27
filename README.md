# Analyze the positive and negative of comments

### Overview 
* Crawled, preprocessed and built an ML method to identify positive or negative comments.
* Improved the accuracy of the Long Short Term Memory model by **15%** using exception handling with **IQR**.
* The result reaches **90%** for *Vietnamese* words, verified by the accuracy of the test set and model metrics

### Dataset

Data is crawled from YouTube and some famous forums of Vietnam.

Dataset includes 2377 sentences labeled with **0 (negative)** and **1 (positive)**

### Preprocessing 
#### IQR
Using IQR to remove the too long or too short sentences

[IQR Wifi](https://en.wikipedia.org/wiki/Interquartile_range)

#### TF-IDF
TF-IDF (term frequency-inverse document frequency) is an information retrieval technique that helps find the most relevant documents corresponding to a given query.

TF is a measure of how often a phrase appears in a document, and IDF is about how important that phrase is. The multiplication of these two scores makes up a TF-IDF score.

[TF-IDF Scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html)


### Model
The model is builts with an embedding layer and an FC layer. The activation function **sigmoid** is used.

### Results
The result reaches **90%** for *Vietnamese* words, verified by the accuracy of the test set and model metrics

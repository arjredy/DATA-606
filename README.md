# DATA-606 Capstone Project on Sentiment Analysis on Yelp Data Reviews
1.Initially, the datasets are downloaded from https://www.yelp.com/dataset. <br>2.As all the datasets are of huge size, each dataset is split into 2 files. Business.csv is only a single file as its file size is below 25MB.

<h3>Read_Json.ipynb:</h3>
1. For the project only Business and Reviews datasets are used. Which are in the form of JSON. By using JSON loads, Reviews and Business datasets are converted into CSV format.<br>
2. Based on Business ID, we merge both the review and business files to obtain the final_data.

<h3>EDA_and_Initial_models.ipynb</h3>
1. By using final_data, perform cleaning on data by using features. Later, basic EDA is performed and features csv (final_full_features.csv) file is generated. <br>
2. By using the features files, initial models are developed. The initital models are LGBM and Cat Boost Classifier.

<h3> LinearSVM.ipynb</h3>
1. By using final_full_features.csv file, and performing text classification and vectorization, on the data, full_tfidf_data.csv will be generated to perform modelling on the whole data using Linear SVM model.

<h3>LinearSVM_Restaurants.ipynb</h3>
1. By using filters, restaurants reviews are taked into separate file.Features are generated into restaurant_features.csv file. Text classification and vectorization are performed on the data to obtain restaurant_tfidf_data.csv. <br>
2. Same Linear SVM model is performed on the restaurants data. A single restaurant business ID is taken to make analysis on research question.

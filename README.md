Scaling of Predicting Taxi fares using distributed machine learning.
Project Overview
The results of this project are a scalable taxi fare prediction model created with distributed
machine learning via PySpark MLlib on the 2023 NYC Yellow Taxi data of January. The goal is
to assess the scalability of various regression algorithms to the big data setting and also compare
the distributed learning with a single node baseline. Mini machines in model are usually unable
to handle transportation data: lots of rows (millions) hence Apache Spark is applied to support
efficient parallel processing, memory optimisation and scalable analytics.
Methodology
The pipeline starts with data ingestion that is Parquet and the subsequent cleaning of data, feature
engineering, as well as vehicle assembly. The major predictors are the distance of tripping, the
number of passengers, the characteristics of pickup times, and the location. To facilitate the
reproducibility the dataset is randomly divided into 80% and 20% training and testing
respectively.
The application of the PySpark MLlib runs four regression models, namely, the Linear
Regression, Decision Tree, Random Forest, and Gradient Boosted Trees (GBT). CrossValidator
is utilized in the hyperparameter tuning. Root Mean Square error (RMSE) and R2 are used to
determine the model performance. Single-node scikit-learn Random Forests randomized on 5%
samples.
Results
The predictive performance of Gradient Boosted Trees (RMSE [?] 6.77, R2 [?] 0.85) is highly
superior and much higher in comparison with Linear Regression. The results confirm that the
ensemble tree-based models are useful in the capture of nonlinear relationships of fare in large
scale taxi data.
Business Value
Tableau dashboards will offer answers to the accuracy of prediction, validation of the pipeline
and the stability of inference at the conclusion of a large scale. The solution assists in the
enhancement of fare forecasting, revenue tracking and also the urban transport planning based on
data.
Conclusion

In this repository, an end-to-end distributed machine learning system is shown, which can work
with more than three million records and be scaled in an efficient manner. The project
emphasizes the significance of the scalable ML pipelines to the real-life smart transportation
analytics.

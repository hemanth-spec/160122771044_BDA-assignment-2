

**Description:**

This Jupyter Notebook contains Python code that demonstrates several applications of Apache Spark's machine learning library (MLlib).  It includes examples of:

* **Recommendation Engine using ALS (Alternating Least Squares):** The code builds a movie recommendation system. It attempts to load movie ratings data from a URL but falls back to using sample data if the URL load fails.  It then trains an ALS model, evaluates its performance, and generates movie recommendations for users and user recommendations for movies.
* **Clustering using KMeans:** This section performs clustering on the Iris dataset (or a sample subset if the URL load fails). It prepares the data, scales the features, applies the KMeans algorithm, and evaluates the clustering.
* **Repeated Recommendation Engine Example:** There's a duplicate of the recommendation engine code, essentially repeating the first example.

**Key Libraries Used:**

* `pyspark.sql` (for Spark DataFrames)
* `pyspark.ml.recommendation.ALS` (for the ALS recommendation model)
* `pyspark.ml.evaluation.RegressionEvaluator` (for evaluating the recommendation model)
* `pyspark.ml.feature.VectorAssembler`, `pyspark.ml.feature.StandardScaler` (for data preparation in clustering)
* `pyspark.ml.clustering.KMeans` (for the KMeans clustering model)
* `pyspark.ml.evaluation.ClusteringEvaluator` (for evaluating clustering)
* `pyspark.ml.Pipeline` (for creating ML pipelines)
* `pyspark.sql.Row` (for creating DataFrame rows)

**Observations:**

* The notebook includes error handling to use sample data if loading data from URLs fails.
* The recommendation engine code is duplicated.
* The clustering example attempts to use the Iris dataset from a URL but also has sample data as a fallback.

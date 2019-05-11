
<h2>Problem statement:</h2>
This project is based on social media link prediction whether two users are going to be friend in future or not.

<h3>Data Overview</h3>
Taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting
data contains two columns source and destination eac edge in graph

- Data columns (total 2 columns):  
- source_node         int64  
- destination_node    int64  

<h3>Mapping the problem into supervised learning problem:</h3>

Generated training samples of good and bad links from given directed graph and for each link got some features like no of
followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc.
and trained ml model based on these features to predict link.

<h3>Business objectives and constraints:</h3>

No low-latency requirement.
Probability of prediction is useful to recommend ighest probability links.

<h4>Performance metric for supervised learning:</h4>
Both precision and recall is important so F1 score is good choice Confusion matrix.

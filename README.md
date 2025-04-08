# SmartSuggest
SmartSuggest is a hybrid recommendation system that uses Singular Value Decomposition (SVD) as collaborative filtering and Hit Ratio estimation as recommendation accuracy, and utilizes review helpfulness scores, user reliability, and clustering coefficients in the review network to quantify user influence.

# Core Idea
Traditional collaborative filtering methods overlook user trust and the contextual value of reviews. SmartSuggest augments SVD-based predictions by quantifying a user's influence and reliability within the network, providing more robust and accurate recommendations

# Dataset used 
We’ve used the amazon data: https://jmcauley.ucsd.edu/data/amazon/index_2014.html, where we focused mainly on “Cell Phones and Accessories”. We divided the dataset and worked on it individually in the following manner : 
	1-188073 :  Anisha Mishra\
  	188074 -376147 : Ankita Satapathy\
  	376148- 564221 : Asipu Khitesha\
  	564222-752295 : Barsha Baibhabi\
  	752296 - 940369 : Barsha Sahoo\
  	940370- 1128437 : Vanshika Raghuvanshi
  
# Requirements
Ensure the following libraries are available:
  pandas
  numpy
  scikit-learn
  networkx
  
# How to Run
- Proceed with SmartSuggest.ipynb to integrate additional user-based features and finalize various scores.
- Analyze the outputs in final_scores1.csv for system results.
- Start by executing SVD_and_HitRatio.ipynb to compute baseline SVD predictions and Hit Ratio evaluation.
  
# Repository Structure
SmartSuggest
├── SmartSuggest.ipynb             # Main pipeline integrating all features and metrics\
├── SVD_and_HitRatio.ipynb         # SVD implementation and Hit Ratio evaluation\
├── reliability_scores.csv         # Precomputed reliability scores per user\
├── final_scores1.csv              # Has final score calculation based on clustering coefficient and the reliability scores\
├── README.md                      # This file

# Features
1. Hybrid Recommendation Model combining:
	- Collaborative Filtering (SVD)
	- Trust-aware and influence-aware metrics
2. User Reliability Estimation
	- Based on consistency and helpfulness of reviews
3. Clustering Coefficients
	- Captures user connectivity in the review network
4. Review Helpfulness Analysis
	- Weighs reviews based on perceived value
5. Performance Evaluation
	- Using Hit Ratio to validate top-N recommendation accuracy












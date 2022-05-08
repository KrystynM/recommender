# Recomender
## Project description

Project is a recomender for hotel reservations whose main goal is to achieve 
the best HR@10 result in the final evaluation. 
The task contains:
- data preprocessing
- prepare user features and item features
- code the recommender
- tune and validate

## Packages
- pandas
- numpy
- seaborn
- IPython
- sklearn
- hyperopt
- matplotlib

## Results
| Description |Recommender|Tune method| HR@10 ||
|-|-|-|-|-|
|For comparison|AmazonRecommender||0.185336||
|Best results|Content-based recommender|SVRCBUIRecommender|0.033944|User featers - average value for user interaction|
|Different approach|Content-based recommender|XGBoostCBUIRecommender|0.029871|User featers - whether the user interact with features|


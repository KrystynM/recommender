# Recomender

## Project description

This project is a recomender for hotel reservations which main goal was to train a content based recommender and achieve the best HR@10 result in the final evaluation.
The task contains:

- data preprocessing
- preparing user features and item features
- coding the recommender
- tuning and validating

Finally, the best results were obtained using SVRCBUIRecommender, for User features calculated by user interaction ratio and one-hot encoding for items.

## How to launch

1.  Install Anaconda with Python 3.8.
2.  Clone the repository
3.  Prepare your conda environment

    1.  Open Anaconda Prompt as administrator.
    2.  Make sure you're in the repository main folder. Run the following command:

            	conda env create --name rs-class-env -f environment.yml>

        You can replace rs-class-env with your own environment name.

4.  In Git Bash open the repository folder and activate just created environment with the following command:

        conda activate rs-class-env

5.  In Git Bash type:

        jupyter notebook

## Results

|     |                    | Recommender            | HR@10    | Description                                               |
| --- | ------------------ | ---------------------- | -------- | --------------------------------------------------------- |
| 1   | Best results       | SVRCBUIRecommender     | 0.033944 | Interaction ratio for user and One-hot encoding for items |
| 2   | Different approach | XGBoostCBUIRecommender | 0.029871 | Best results using one-hot encoding for items and users   |
| 3   | For comparison     | AmazonRecommender      | 0.185336 |                                                           |

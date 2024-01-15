# NBA MVP Voting
In this project, we used an NBA MVP voting dataset from Kaggle (https://www.kaggle.com/datasets/vivovinco/19912021-nba-stats) and trained 2 different models that predict how many points a player would receive given some variables.

# Exploratory Data Analysis
To begin, we first did some Exploratory Data Analysis on the dataset to see any correlations that some variables had on others. After creating and examining a Correlation Heatmap, a Scatter Plot, and a Boxplot, we decided to have the "Pts Won" column as our target variable and the "First", "Rank", and "Share" columns as our predictors. Although we didn't realize it until the very end of our project, our predictors were dependent variables, which should not be the case.

# Preprocessing phase
Next, we moved onto the preprocessing phase, where we encountered some errors when loading the dataset. Although there were no null values, the names of players with an accent mark were getting replaced with a question mark. To fix this, we discovered where and who's names were being edited, then created a dictionary to replace the names read in into their actual names. Luckily, there weren't a lot of players with this error (only 4), so the process didn't take too long. Also, we decided to label encode the "Rank" column to become numerical values so that we could apply our models to it.  

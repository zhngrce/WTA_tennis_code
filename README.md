# WTA_tennis_code
Code for Pioneer Data Science Research.

# Steps Done
1. Import dataset: WTA matches up until July 3, 2023 (https://zenodo.org/record/8174943)

   Dataset of 2017-2023 matches used: https://docs.google.com/spreadsheets/d/1WlTc3stL8WRWqkix1m68OQ2H-A-CkC_Zl9sjWX6kuIg/edit?usp=sharing
   
3. Light dataset cleaning
4. Read CSVs: tournament-level correlation and level-points correlation
   
   Tournament-level correlation: https://docs.google.com/spreadsheets/d/1IMXMYlZgRn_xMLRINCQ9t4tRKDMxePx33gA_QssOYBA/edit?usp=sharing

   :Level-points correlation: https://docs.google.com/spreadsheets/d/1NZmOS_vVzJylOKGU0uQQKE6UrYzvn7DYsZFgLHCss_U/edit?usp=sharing
   
## Simple Model
4. Simulate total rankings for simple models
5. Simulate surface-specific rankings for simple models
6. Evaluate accuracies for total and surface-specific rankings on sub-datasets

## Decision Tree
7. Create sub-datasets for decision trees
8. Create hard, clay, grass-only datasets
9. Simulate total, hard, clay, grass rankings with number of points and number of matches for each player
10. Add dataframe of total and surface rankings to dataframe of matches; data added depends on decision tree type
11. Drop columns with information that is not used in decision tree calculations (tournament name and date, winner and loser id, etc.)
12. Randomize winner and loser index, creates a separate list with the index of the winner
13. Convert categorical data to numerical data (round, surface)
14. Remove winner index from X_train and X_test dataframes; create Y_train and Y_test out of winner index column
15. Use decision tree classifier from scikit-learn to predict winner and evaluate accuracy 


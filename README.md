# kaggle-titanic

##Kaggle - Titanic - Machine Learning from Disaster

Entry for Kaggle competition - https://www.kaggle.com/competitions/titanic/overview


## Submission 1

This was my first attempt and just did some basic mutual information analysis and selected parameters from there.
Notebook can be found [here](src/submission-01.ipynb).

Submissions score was `0.77511`

## Submission 2

After reviewing some other notebooks (notably this [one](https://www.kaggle.com/code/dhruvinkakadia/titanic-survival-classifier-top-2/notebook?scriptVersionId=87264651)) I have a few other things I want to try:

- Break ages into bins - Done
- Break fares into bins - Done
- Change SibSp into a 0/1 attribute. If people are alone or with family - Done
- Change ParCh into a 0/1 attribute. If people are alone or with family - Done
- look at adding a deck feature - Done
  - There are quite a few unknown so that can be its own category
  - We may need to group decks with similar properties and/or low numbers
- one-hot embarked
  - for people without embarked
    - We could just use the most common?
    - Or based on their fare, select the embarkation location
- Also look at trying some different model

- Possible improvements:
  - Test changing SibSp, ParCh, Sex and Cabin to one-hot
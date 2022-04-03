# Kaggle - Titanic - Machine Learning from Disaster

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

This ended up with an identical score `0.77511`. Submission notebook [here](src/submission-02.ipynb)

## Final(?) notes

After doing some research it appears that any score above 75% is a reasonably good one. The highest every acheived was 83%. There is likely some more processing that could be done to offer some better data/results:

- One-hot embarked, sex
- Calculate total family size
- Have a feature for a women with children as this was apparently an indicator of likely death.

However, I'll leave this for now as it was a good learning project and may also not be worth putting in hours more work to achieve a few more percent accuracy. I may revisit this in the future once I've learned more to see if I can improve.
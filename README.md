# Competitive League of Legends Game Winner Prediction

![](data/images/icon.jpg)

## Introduction

LoL is an online, 5 vs. 5 competitive PC game. It is one of - if not the most - popular game currently around. Despite that LoL has surprisingly little mainstream coverage, which is most likely due to its complexity - it’s not an easy game to understand.

LoL has a professional league. The top prize for the best team is over five million dollars and the average player makes a six-figure income. This data set aggregates basic statistics for every game since 2015 across all the professional leagues other than China.

![](data/images/map.jpg)

## Datasets

We have an available dataset on kaggle for model training, the dataset includes competitive matches from 2015 to 2017. The matches include the NALCS, EULCS, LCK, LMS, and CBLoL leagues as well as the World Championship and Mid-Season Invitational tournaments :
- https://www.kaggle.com/datasets/chuckephron/leagueoflegends?resource=download

Riot games also provides an API from which we can fetch more actual data :
- https://developer.riotgames.com/apis

## Objective: Predicting the Winner of Competitive League of Legends Matches

The primary goal of this project is to develop a model that predicts the outcome of competitive 5v5 League of Legends matches. More than just a static pre-game prediction, the model should dynamically update the probability of winning as the game progresses, incorporating key events and game state changes.

### Key Phases of Prediction Updates:

- Champion Select & Ban Phase – Certain team compositions or meta-relevant champions may significantly impact win probability before the match even starts.
- Early Game Events – The first few minutes can heavily influence momentum:
  - First Blood (the first kill) provides an early gold and psychological advantage.
  - First Tower grants significant gold and better map control.
- Mid to Late Game Factors – Real-time tracking of key statistics such as:
  - Gold Difference – A leading indicator of overall team strength.
  - Kill Difference – Reflects combat dominance and potential snowballing.
  - Other Key Metrics (e.g., vision control, Baron/Dragon takes, turret count) could also be considered for improving prediction accuracy.

By continuously refining win probability based on these events, the model aims to provide real-time insights into a team's chances of winning as the match unfolds.

Useful link -> https://www.kaggle.com/discussions/general/330263

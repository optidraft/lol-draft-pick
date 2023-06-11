# UCI Capstone Project
## League of Legends: Draft & Pick

This is the capstone project of the UCI Data Science undergraduate course, under the courses Stats170A and Stats170B, with two professors, Babak Shahbaba and Faisal Nawab, as the instructors. We are the Team 10 of the 2023 Graduation Capstone Project. The members who completed the project include Yuan Zhang ([@yuanzzhang](https://github.com/yuanzzhang)), Hongqu Shi ([@Wi1lShi)](https://github.com/Wi1lShi), Jingjing Xu ([@Jessicaaaa2](https://github.com/Jessicaaaa2)), Xiaomeng Ren ([@xiaomeng0120](https://github.com/xiaomeng0120)), Boya Shao ([@boyashao](https://github.com/boyashao)).

Our goal is to develop a system to predict the win rate of a game in League of Legends (LoL), based on the champions chosen by the player, the lineup of opposing players, and the champions banned by both players. To ensure compatibility with evolving game versions, we focused our research on two specific versions: 10.16 (60k LoL matches) and 13.9 (36k LoL matches). We hope to provide players with reasonable predictions of the battle situation as a reference through a large amount of data research on these two versions.



## Project Pipeline

[Collect data](https://github.com/optidraft/lol-data-collection)-->[Extract tables](https://github.com/optidraft/lol-draft-pick/blob/main/notebooks/v13.9/data_extract.ipynb)-->[Compute synergy score](https://github.com/optidraft/lol-draft-pick/blob/main/notebooks/v13.9/synergy_score.ipynb)-->[Train models](https://github.com/optidraft/lol-draft-pick/blob/main/notebooks/v13.9/model_form.ipynb)-->[Deploy web user interface](https://optidraft.github.io/optidraft/)

Simplified project demo: `project.ipynb`


## Project Directory

```
lol-draft-pick/
├── .gitignore
├── data/
│   └── 13data.csv                  # data for training models
├── models/                         # saved models
│   ├── mlp.joblib
│   └── rf.joblib
├── notebooks/
│   ├── v10.16/                     # game version: 10.16
│   │   ├── data_extract.ipynb      # data wrangling
│   │   ├── model_form.ipynb        # train models
│   │   └── synergy_score.ipynb     # compute synergy score
│   └── v13.9/                      # newer game version: 13.9
│       ├── data_extract.ipynb
│       ├── model_form.ipynb
│       └── synergy_score.ipynb
├── project.html                    # demo html file
├── project.ipynb                   # demo models
└── README.md
```



# MTS Kion Implicit Contextualised Sequential Dataset for Movie Recommendation

## Dataset Description
This is an official repository of the Kion Movies Recommendation Dataset

The public part of the  dataset includes 5,476,251 interactions of 962,179 users with 15,706 items. The dataset includes user-item interactions; users demographics and rich items meta-data. 

*Private* part of the dataset is not released to general public, however there is a public sandbox, where the researchers can measure MAP@10 metric on the private part of the data. 

Sandbox is accessible by the address https://ods.ai/competitions/competition-recsys-21/leaderboard/public_sandbox



### The dataset consists of three parts: 
1. **Interactions.csv** - contains user-item implicit interactions, watch percentages, watch durations
2. **Users.cvs** - contains users demographics information (sex, age band, income level band, kids flag) 
3. **Items.cvs** - contains items meta-information (title, original title, year, genres, keywords, descriptions, countries, studios, actors, directors)

#### The users and items files have two versions: 

* **data_original** - original meta-information in Russian language
* **data_en** - english version of the metadata translated with Facebook FAIR’s WMT19 Ru->En machine translation model. 

## Comparison with MovieLens-25M and Netflix datasets

### Quantitative comparison:
|                              | **Netflix** |**Movielens-25M** | **Kion**           |
|------------------------------|-------------|------------------|--------------------|
| Users                        | 480,189     | 162,541          | 962,179            |
| Items                        | 17,770      | 59,047           | 15,706             |
| Interactions                 | 100,480,507 | 25,000,095       | 5,476,251          |
| Avg. Session Length          | 209.25      | 153.80           | 5.69               |
| Sparsity                     | 98.82%      | 99.73%           | 99.9%              |


### Qualitative comparison: 
| **Dataset Name**                       | **Netflix**.        |       **Movielens-25M**                  | **Kion**                        |
|----------------------------------------|---------------------|------------------------------------------|---------------------------------|
| Type                                   | Explicit (Ratings)  | Explicit (Rating)                        | Implicit (Interactions)         |
|         Interaction registration time. | After watching      | After watching                           | At watching                     |
|         Interaction features           | Date, Rating        | Date, Rating                             | Date, Duration, Watched Percent |
|         User features                  | None                | None                                     | Age, Income, Kids               |
|         Item features                  | Release Year, Title |Release Year, Title, Genres, Tags           | Content Type, Title, Original Title, Release Year, Genres, Countries, For Kids, Age Rating, Studios, Directors, Actors, Description, Keyword |

# Kion challenge
This dataset was used for the Kion challenge recommendation contest [ (Official website in Russian Language)](https://ods.ai/competitions/competition-recsys-21). 

This table contains results of the winners of the competition, measured on the private part of the dataset: 

| Position            | Name              | MAP@10 | Solution Type                  |
|---------------------|-------------------|--------|--------------------------------|
| 1                   | Oleg Lashinin     | 0.1221 | Neural and Non-Neural ensemble |
| 2                   | Aleksandr Petrov  | 0.1214 | Neural and Non-Neural ensemble |
| 3                   | Stepan Zimin      | 0.1213 | Non-Neural ensemble            |
| 4                   | Daria Tikhonovich | 0.1148 | Gradient Boosting Trees        |
| 5                   | Olga              | 0.1135 | Gradient Boosting Trees        |
| Popularity baseline |                   | 0.0910 |                                |


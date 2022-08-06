# MTS Kion Implicit Contextualised Sequential Dataset for Movie Recommendation

## Dataset Description
This is an official repository of the Kion Movies Recommendation Dataset

The public part of the  dataset includes 5,476,251 interactions of 962,179 users with 15,706 items. The dataset includes user-item interactions; users demographics and rich items meta-data. 

*Private* part of the dataset is not released to general public, however there is a public sandbox, where the researchers can measure MAP@10 metric on the private part of the data. 

Sandbox is accessible by the address https://ods.ai/competitions/competition-recsys-21/leaderboard/public_sandbox



### The dataset consists of three parts: 
1. Interactions.csv - contains user-item implicit interactions, watch percentages, watch durations
2. Users.cvs - contains users demographics information (sex, age band, income level band, kids flag) 
3. Items.cvs - contains items meta-information (title, original title, year, genres, keywords, descriptions, countries, studios, actors, directors)

#### The users and items files have two versions: 

data_original - original meta-information in russian language
data_en - english version of the metadata translated with Facebook FAIR’s WMT19 Ru->En machine translation model. 





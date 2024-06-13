# Poli179-Final-Project
## Research Question
During significant international conflicts involving the U.S. in history, is there an increase in the racist language towards non-U.S. groups in conflict appearing in the content of the article?
## Overview
We will be measuring whether “racist language” arises in articles during U.S. international conflict with specifically foreign states. To measure “racist language,” we will be examining the implicit stigmatization with coded language or language that subtly insinuates racist sentiments. For each conflict, we will find the number of times racist language is used towards ethnicities involved during a given year during the time of the conflict versus the presence of racist language not during the time of the conflict. To analyze the number of times racist language is used when there is no conflict, we will run the same tests on surrounding years and average out their frequencies to find the average amount of racist language during a non-conflict year. We will repeat this process for multiple major conflicts and use regression to find if there is a relationship between space in time (conflict year vs. non conflict year) and the frequency of racist language.

## Conceptual Framework 
Similarly to the theoretical design of Müller et. al’s study, we are operating under the established notion that “individuals’ explicit and implicit judgments of the same groups can vary.” 
While explicit stigmatization often takes on a substantial and overt form of discrimination, the subtle implications from implicit stigmatization may still be as influential on shaping attitudes through a subconscious form. Hence, to discern between the two stigmatizations, we will focus on how often implicit stigmatization may arise in news coverage because the context of war may play an effective role in proliferating the rate that discrimination may occur.  

The U.S.'s involvement in international conflict has been a significant facet of the nation's history, especially knowing the historical context of 20th century wars. Hence, the wars we will inspecting in this project are: Mexican Border War, World War I, Russian Civil War, World War II, and the Korean War. Considering American history, the overt discrimination taking form as racial charicatures and other stereotypes has been commonly understood as an explicit discrimination for framing opposing groups; yet, we aim to examine the extent that subtle insinuations of discrimination arises during war times, and whether this intertwines with framing social identity rhetoric to exacerbate racial divisions similarly to explicit discrimination. By examining the extent of discrimination that the people of the opposition side may be facing during conflict years versus non-conflict years, the historical context signifies how implicit insinuations of discrimination may also play a key role in shaping social attitudes. 

As a theoretical foundation for our project, we are interested in how conflict leads to identity discrimination in the media. During significant international conflicts, social attitudes may be highly impressionable on fostering discrimination due to the tensions involving violent, militaristic conflict. When the media becomes involved in shaping these attitudes, we are interested in how often the media tends to frame stories in a certain way to exacerbate these negative attitudes through racist language. Thus, here are key terms we will be utilizing in our study:
{\begin{itemize}
     \item Implicit stigmatization: language that discriminates against individuals based on race, ethnicity, and/or national identity; this may manifest as slurs, stereotypes, and derogatory terms. 
    \item Racist language: coded language or language that subtly insinuates racist sentiments
    \item International conflict: military or political altercation involving the U.S. and other countries; this may be World War I, Korean War, and World War II. 

\end{itemize} 
}
Given this conceptual framework, our guiding hypothesis of this study is: during a conflict year, we predict that there is more racial stigmatization against non-U.S. groups compared to non-conflict years. 
## Methods
1. We clean the data by removing the unwanted columns
2. Use BERT for tokenizing then embedding the articles
3. establishing a preset list of racist words as the keywords, then encoding those racist keywords.
4. finding the cosine similarity between the embedded articles and the embedded keywords
5. compare the cosine similarity of a year in the conflict versus a year not in the conflict.
6. use a regression to model the pattern of behavior through different conflicts.
## Current Limitations
We are having trouble with processing our data because of how large the dataset is. We wanted to first analyze all data from the 20th century as a whole and do the embeddings with that data set, but there were way too many articles to analyze and our computers couldn't load all of it at once. So our current plan is to do the analysis on each conflict individually by picking a year during that conflict and a year not during that conflict and doing the embeddings just on those years instead of grouping together the whole 20th century. When I run the code that encodes the articles for the year of the mexican border conflict, it was running 30 minutes before I had to turn off my computer to go to class. We're not sure if we should reduce the number of articles somehow, or if it is something that we should change with our code to allow for more efficient running.

*The Code that has been done so far is in the notebook folder under 01_data_cleaning(1).ipynb

https://colab.research.google.com/drive/1fHvxHgzGC5C1Zb5839Gw6DHAMWKaMSSb?usp=drive_link

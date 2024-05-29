# Poli179-Final-Project
Research Question: 
During significant international conflicts involving the U.S. in history, is there an increase in the racist language towards non-U.S. groups in conflict appearing in the content of the article?
Overview:
We will be measuring whether “racist language” arises in articles during U.S. international conflict with specifically foreign states. To measure “racist language,” we will be examining the implicit stigmatization with coded language or language that subtly insinuates racist sentiments. For each conflict, we will find the number of times racist language is used towards ethnicities involved during a given year during the time of the conflict versus the presence of racist language not during the time of the conflict. To analyze the number of times racist language is used when there is no conflict, we will run the same tests on surrounding years and average out their frequencies to find the average amount of racist language during a non-conflict year. We will repeat this process for multiple major conflicts and use regression to find if there is a relationship between space in time (conflict year vs. non conflict year) and the frequency of racist language.
Methods:
1. We clean the data by removing the unwanted columns
2. Use BERT for tokenizing then embedding the articles
3. establishing a preset list of racist words as the keywords, then encoding those racist keywords.
4. finding the cosine similarity between the embedded articles and the embedded keywords
5. compare the cosine similarity of a year in the conflict versus a year not in the conflict.
6. use a regression to model the pattern of behavior through different conflicts.
Troubles So Far:
We are having trouble with processing our data because of how large the dataset is. We wanted to first analyze all data from the 20th century as a whole and do the embeddings with that data set, but there were way too many articles to analyze and our computers couldn't load all of it at once. So our current plan is to do the analysis on each conflict individually by picking a year during that conflict and a year not during that conflict and doing the embeddings just on those years instead of grouping together the whole 20th century. When I run the code that encodes the articles for the year of the mexican border conflict, it was running 30 minutes before I had to turn off my computer to go to class. We're not sure if we should reduce the number of articles somehow, or if it is something that we should change with our code to allow for more efficient running.


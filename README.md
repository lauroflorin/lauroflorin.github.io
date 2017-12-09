<iframe width="854" height="480" src="https://www.youtube.com/embed/tyh07c5I7eU" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>
<span class="credits right"><a class="tar_download_link" href="Explainer_notebook.ipynb">View Explainer Notebook</a>   |   <a class="zip_download_link" href="./Explainer_notebook.ipynb">Download datasets(.zip)</a></span>
# Motivation
We want to find out if humans have discovered yet that lab rats and dolphins are smarter than them so our question is: who’s the smartest animal in town? Our team decided that the best way to find out was to search the dark deep web of Facebook.


 __Choice of dataset__

Upon a search for the most relevant Facebook groups, 3 stood out (most members, >5000): Animal Cognition, Anthrozoology and Animal Cognition, the Emotional and Intellectual Lives of Animals. Our assumption is that everything posted on these groups is scientific and related to the intelligence of animals (due to the groups' names), so therefore if a post on these groups mentions an animal, that animal must be smart. 


# Basic stats about the dataset

After using Facebook's API to download all the required materials, we ended up with the following datasets:

* __Animal Cognition:__
    - 6 956 posts
    - 4726 members
    - 9779 comments
    - 11887 mentioned animals


* __Animal Cognition, the Emotional and Intellectual Lives of Animals:__
    - 10 364 posts
    - 4825 members
    - 7928 comments
    - 15316 mentioned animals


* __Anthrozoology:__
    - 7 442 posts
    - 3200 members
    - 13750 comments
    - 9331 mentioned animals

* 24 762 posts in total, 78.3 MB of pickles

Also, Wikipedia was mined for a list of animals by common name. This list was chosen because it seemed the most relevant, as people mention animals by their common name (as opposed to the scientific one) when posting about them on facebook.


# Sentiment analysis

* We performed sentiment analysis on the text in the posts, in order to get a feeling of how people perceive the different animals.
* For performing sentiment analysis we used the The LabMT 1.0. (‘language assessment by Mechanical Turk 1.0’) list, which was created with the use of Amazon Mechanical Turk, which is a crowdsourcing service that provides 'human intelligence'. The top 5000 most frequent words from 4 sources (Twitter, Google Books, music lyrics, and the New York Times) were merged in a set of 10 222 words. These words were rated by users of Amazon Mechanical Turk, based on their _average happiness_, from 1 to 9.

 * By computing the average of all the words in all the posts in each group, we were able to determine the average sentiment of the 3 groups:
 
| Group        | Average Sentiment |
| ------------- |:-------------:|
| Animal Cognition     | 5.54518814266  |
| Animal Cognition, the Emotional and Intellectual Lives of Animals|5.56189498169     |
| Anthrozoology | 5.5083218857 | 

It turns out, people are optimistic when talking about animal intelligence, since the happiness of each group is above average.


* When performing sentiment analysis for each animal, these were the top animals:

![alt text](images/top_20_anthrozoology.png)


![alt text](images/top_20_animal_cog.png)


![alt text](images/top_20_animal_cog_and_em.png)

When looking at the last 20 animals in the happines ranks, we notice that they aren't very far from the top ones. From this we drew the conclusion that when people post or talk about an animal in these groups, it is mostly positive things.



![alt text](images/last_20_anthrozoology.png)


![alt text](images/last_20_animal_cog.png)


![alt text](images/last_20_animal_cog_and_em.png)

# Lexical Dispersion

* We were interested to see if there is a pattern in how the animals appear in posts throughout time.
* We sorted all the posts by date (from 2012 until present), then used the _dispersion\_plot_ method from the _nltk_ library. We checked for the first 50 animals most often encountered in the stemmed and tokenized text from all posts.
* The lexical dispersion plot looks very similar for the three groups and it is more or less constant, with some burstiness at some animals (for example  _bear_ and _lion_ in the graph below).

![alt text](images/lex_disp_animal_cog_and_em_ed.png)

# Collocations

* We checked for collocations to see if there are similarities in how people discuss about this subject, the intelligence of other animals.
* We also used in this analysis the method _collocations_ from the _nltk_ library applied to the tokenized text, concatenated from all posts.
* Some of the collocations turned out to be expressions that are very relevant to animal cognition and the way people feel and talk about animals such as:

   * non human
   * first time
   * facial expressions
   * animal cognition 
   * decision making
   * problem solving
   * self awareness
   * great apes
   * current biology
   * nonhuman animals
   * cognitive abilities
   * mirror test
   * nervous system
   * feel pain
   * animal behaviour
   * best friend
   * climate change
   * wildlife service
   * critically endangered
   * sea turtle
   * good article
   * animal rights
   * intellectual lives

* Some other types of collocations showed that a lot of people research what they are posting about and talk about relevant sources:

   * scientist magazine
   * paper published
   * previously thought
   * study finds
   * scientific american
   * state university
   * peer reviewed
    
* Another thing we discovered was that in one of the groups, anthrozoology, there are a lot of Spanish speaking members, since a lot of the collocations are in spanish (los animales, perseguir lasl, las palabras etc.)
  
  # Top posters in each group
  
  * We checked for the members with the most posts, reactions and overall interactions (posts + reactions + comments) to get more info on how the people in the group behave.
  
  
  __Animal Cognition:__
  
  
  |    |Name                     | Number of comments| Number of posts| Number of Reactions| Total interactions
  |----|----                     |--------------------|---------------|--------------------|--------------------|
  |Most Posts|Robert Karl Stonjek|1120|3070|20|4210|
  |Most Reactions|Dmitri Kaminiar|28|366|2886|3280|
  |Most Comments|Robert Karl Stonjek|1120|3070|20|4210|
  |Most Interactions|Robert Karl Stonjek|1120|3070|20|4210|
  
  * In this group there are 2 dominant members who take part in most of the interactions and discussions.

  __Animal Cognition and Emotional Intelligence:__
  
  
  |    |Name                     | Number of comments| Number of posts| Number of Reactions| Total interactions
  |----|----                     |--------------------|---------------|--------------------|--------------------|
  |__Most Posts__|Susan Freeman|5514|21555|4059|31128|
  |__Most Reactions__|Susan Freeman|5514|21555|4059|31128|
  |__Most Comments__|Susan Freeman|5514|21555|4059|31128|
  |__Most Interactions__|Susan Freeman|5514|21555|4059|31128|
  
  * In this group we were surprised to see that there is only one person who does most of the posting, reacting and commenting.

  __Anthrozoology:__
  
  
  |    |Name                     | Number of comments| Number of posts| Number of Reactions| Total interactions
  |----|----                     |--------------------|---------------|--------------------|--------------------|
  |__Most Posts__|Manuel Fernandez Albores|270|1656|832|2758|
  |__Most Reactions__|Gala Argent|930|344|2994|4268|
  |__Most Comments__|Gala Argent|930|344|2994|4268|
  |__Most Interactions__|Piers Locke|1178|1486|1642|4306|
  
* In this group, we weren't surprised to see that the top poster was _Manuel Fernandez Albores_, since most of the collocations we found when analysing the text were in Spanish and he has a Spanish-sounding name.

# Top posters in all groups

* We also did the intersection of the members between the three groups, to see if we find any of the winners from the previous categories, who are being active in more than one group:

  |    |Name                     | Number of comments| Number of posts| Number of Reactions| Total interactions
  |----|----                     |--------------------|---------------|--------------------|--------------------|
  |__Most Posts__|Gala Argent|467|172|1744|2383|
  |__Most Reactions__|LizDonguri Capaldi Capybara|268|155|3134|3557|
  |__Most Comments__|Dennis Low|799|63|86|948|
  |__Most Interactions__|LizDonguri Capaldi Capybara|268|155|3134|3557|
 
* We have found one person who was in the top members in a group and three new persons, which may suggest that most people are only active in one group of their choice.


# Most liked animal in each group and in all groups

* We counted the reactions to the posts of which the animals were subject, to determine which are the most popular animals in each group:

__Top 10 animals__

|Animal Cognition|
|----|
|dog|
|bird|
|cat|
|chimpanzee|
|elephant|
|crow|
|monkey|
|dolphin|
|fish|
|parrot|                           
                                                                               
                                                                                                                                                            
|Animal Cognition and Emotional Intelligence|
|-------------------------------------------|                                                                          
|dog|
|elephant|
|whale|
|bird|
|horse|
|cat|
|dolphin|
|cattle|
|bear|
|fish|
                                                                               
  
  
  
|Anthrozoology|
|-------------|
|dog|
|elephant|
|bird|
|cat|
|horse|
|wolf|
|chimpanzee|
|bear|
|whale|
|fish|

                                                                               
|All 3 groups|
|----------------|
|dog|
|elephant|
|bird|
|cat|
|whale|
|horse|
|chimpanzee|
|dolphin|
|fish|
|bear                                                                                     
                                                                               
* These results were also satisfactory, as these animals are indeed popular in humans' opinions.

# Which group is more qualitative?


* We evaluated this by looking at the type of posts, at how many of the posts have descriptions and how many words users add on each post.
* The results weren't very conclusive, the groups have a very similar distribution of types of posts, most of the posts being links in each group.


                                                                               


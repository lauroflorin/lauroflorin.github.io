<iframe width="854" height="480" src="https://www.youtube.com/embed/tyh07c5I7eU" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>

# Motivation
 We want to find out if humans have discovered yet that lab rats and dolphins are smarter than them so our question is: who’s the smartest animal in town? 


* __Choice of dataset__

We decided that these were the 3 most relevant Groups: Animal Cognition, Anthrozoology and Animal Cognition, the Emotional and Intellectual Lives of Animals. Since these facebook groups are all about science, more specifically the intelligence of animals, our assumption is that if a post on these groups mentions an animal, that animal must be smart.

* __Goal for the end user's experience__
>

# Basic stats about the dataset

The posts from 3 Facebook groups:

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

* Wikipedia was mined for a list of all animals by common name. This list was chosen because it seemed the most relevant, as people mention animals by their common name (as opposed to the scientific one) when posting about them on facebook.


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
    
* Another thing we discovered was that in one of the groups, anthrozoology, there are a lot of Spanish speaking members, since a lot of the collocations are in spanish:

   * los animales
   * perseguir las
   * las palabras
   * las sombras
   * arte zoolog
   * por mafa
   * genes las
   * multidisciplinar docente
   * diversas exposiciones
   * ense anzas
   * sobre arte
    
  
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
  |Most Posts|Susan Freeman|5514|21555|4059|31128|
  |Most Reactions|Susan Freeman|5514|21555|4059|31128|
  |Most Comments|Susan Freeman|5514|21555|4059|31128|
  |Most Interactions|Susan Freeman|5514|21555|4059|31128|
  
  * In this group we were surprised to see that there is only one person who does most of the posting, reacting and commenting.

  __Anthrozoology:__
  
  
  |    |Name                     | Number of comments| Number of posts| Number of Reactions| Total interactions
  |----|----                     |--------------------|---------------|--------------------|--------------------|
  |Most Posts|Manuel Fernandez Albores|270|1656|832|2758|
  |Most Reactions|Gala Argent|930|344|2994|4268|
  |Most Comments|Gala Argent|930|344|2994|4268|
  |Most Interactions|Piers Locke|1178|1486|1642|4306|
  
* In this group, we weren't surprised to see that the top poster was _Manuel Fernandez Albores_, since most of the collocations we found when analysing the text were in Spanish and he has a Spanish-sounding name.

# Top posters in all groups

* We also did the intersection of the members between the three groups, to see if we find any of the winners from the previous categories, who are being active in more than one group:

  |    |Name                     | Number of comments| Number of posts| Number of Reactions| Total interactions
  |----|----                     |--------------------|---------------|--------------------|--------------------|
  |Most Posts|Gala Argent|467|172|1744|2383|
  |Most Reactions|LizDonguri Capaldi Capybara|268|155|3134|3557|
  |Most Comments|Dennis Low|799|63|86|948|
  |Most Interactions|LizDonguri Capaldi Capybara|268|155|3134|3557|
 
* We have found one person who was in the top members in a group and three new persons, which may suggest that most people are only active in one group of their choice.


<span class="credits right"><a class="tar_download_link" href="https://github.com/JW0914/Wikis/tarball/master">tar</a>   |   <a class="zip_download_link" href="https://github.com/JW0914/Wikis/zipball/master">zip</a></span>



<iframe width="854" height="480" src="https://www.youtube.com/embed/tyh07c5I7eU" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>

# Motivation
 We want to find out if humans have discovered yet that lab rats and dolphins are smarter than them so our question is: who’s the smartest animal in town? 


* __Choice of dataset__

We decided that these were the 3 most relevant Groups: Animal Cognition, Anthrozoology and Animal Cognition, the Emotional and Intellectual Lives of Animals. Since these facebook groups are all about science, more specifically the intelligence of animals, our assumption is that if a post on these groups mentions an animal, that animal must be smart.

* __Goal for the end user's experience__
>

# Basic stats about the dataset

The posts from 3 Facebook groups:

* Animal Cognition - 6 956 posts

* Animal Cognition, the Emotional and Intellectual Lives of Animals - 10 364 posts

* Anthrozoology - 7 442 posts

* 24 762 posts in total, 78.3 MB of pickles


# Sentiment analysis

* We performed sentiment analysis on the text in the posts, in order to get a feeling of how people perceive the different animals.
* For performing sentiment analysis we used the The LabMT 1.0. (‘language assessment by Mechanical Turk 1.0’) list, which was created with the use of Amazon Mechanical Turk, which is a crowdsourcing service that provides 'human intelligence'. The top 5000 most frequent words from 4 sources (Twitter, Google Books, music lyrics, and the New York Times) were merged in a set of 10 222 words. These words were rated by users of Amazon Mechanical Turk, based on their _average happiness_, __from 1 to 9. __
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
   
  
  

<span class="credits right"><a class="tar_download_link" href="https://github.com/JW0914/Wikis/tarball/master">tar</a>   |   <a class="zip_download_link" href="https://github.com/JW0914/Wikis/zipball/master">zip</a></span>



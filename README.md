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
* For performing sentiment analysis we used the The LabMT 1.0. (_ ‘language assessment by Mechanical Turk 1.0’_) list, which was created with the use of Amazon Mechanical Turk, which is a crowdsourcing service that provides 'human intelligence'. The top 5000 most frequent words from 4 sources (Twitter, Google Books, music lyrics, and the New York Times) were merged in a set of 10 222 words. These words were rated by users of Amazon Mechanical Turk, based on their _average happiness_, __from 1 to 9. __
 * By computing the average of all the words in all the posts in each group, we were able to determine the average sentiment of the 3 groups:
 
| Group        | Average Sentiment |
| ------------- |:-------------:|
| Animal Cognition     | 5.54518814266  |
| Animal Cognition, the Emotional and Intellectual Lives of Animals|5.56189498169     |
| Anthrozoology | 5.5083218857 | 

It turns out, people are optimistic when talking about animal intelligence, since the happiness of each group is above average.


* When performing sentiment analysis for each animal, these were the top animals:

__Animal Cognition__

|                   animal | happiness |  
| ------------------------ |:---------:|
|               armadillo  | 7.260000  |
|  pufferfish|puffer fish  | 5.883267  |
|             nightingale  | 5.871176  |
|                 mustang  | 5.844286  |
|             sperm whale  | 5.839333  |
| pointer|english pointer  | 5.815962  |
|                 catfish  | 5.813705  |
|                     emu  | 5.798333  |
|                    lark  | 5.786944  |
|             rattlesnake  | 5.766579  |
|                 mollusk  | 5.744444  |
|                 manatee  | 5.743006  |
|                   camel  | 5.733125  |
|               alligator  | 5.708439  |
|                  jaguar  | 5.705831  |
|                    ibis  | 5.703747  |
|               clownfish  | 5.701389  |
|                 asp|asp  | 5.700889  |
|    geococcyx|roadrunner  | 5.698322  |
|                sea lion  | 5.692398  |


Animal Cognition and emotion
             animal  happiness
             jackal   6.223659
               newt   5.952708
          bandicoot   5.940000
   great blue heron   5.936364
         blue whale   5.925807
             limpet   5.885455
   peregrine falcon   5.848571
      thrush|thrush   5.846459
              leech   5.836000
      elephant seal   5.824423
              stork   5.824187
               dove   5.816619
             marten   5.807143
          cockatiel   5.802000
               lark   5.801403
           scorpion   5.800047
               dodo   5.770938
         guinea pig   5.768571
      water buffalo   5.766792
  fennec fox|fennec   5.757500 


Anthrozoology
                    animal  happiness
0                bumblebee   6.118750
1                 platypus   5.916986
2           humpback whale   5.889164
3                dragonfly   5.882108
4                red panda   5.824444
5                cockatiel   5.819310
6                   gibbon   5.787368
7                  mollusk   5.780560
8   pufferfish|puffer fish   5.767458
9                 barnacle   5.761333
10                silkworm   5.756000
11                 asp|asp   5.753169
12                    swan   5.751723
13                  dragon   5.742493
14                  cicada   5.732444
15                   hyrax   5.729677
16              arctic fox   5.710000
17                 ostrich   5.709880
18                   squid   5.705649
19                   egret   5.700500 




<span class="credits right"><a class="tar_download_link" href="https://github.com/JW0914/Wikis/tarball/master">tar</a>   |   <a class="zip_download_link" href="https://github.com/JW0914/Wikis/zipball/master">zip</a></span>



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
__Animal Cognition:__

|Animal      | Average Sentiment |
| ------------- |:-------------:|
|armadillo | 7.26|
|pufferfish| 5.883266883132783|
|nightingale | 5.871176470588235|
|mustang | 5.844285714285715|
|sperm whale | 5.839333333333332|
|pointer | 5.815961538461538|
|catfish | 5.813705357142858|
|emu | 5.798333333333333|
|lark | 5.786944444444444|
|rattlesnake | 5.766578947368419|
|mollusk | 5.744444444444445|
|manatee | 5.74300630149132|
|camel | 5.733125000000002|
|alligator | 5.708438544036948|
|jaguar | 5.705830728061558|
|ibis | 5.703747252747252|
|clownfish | 5.701388888888888|
|asp | 5.700889029003784|
|geococcyx | 5.698322147651006|
|sea lion | 5.692397578347578|





<span class="credits right"><a class="tar_download_link" href="https://github.com/JW0914/Wikis/tarball/master">tar</a>   |   <a class="zip_download_link" href="https://github.com/JW0914/Wikis/zipball/master">zip</a></span>



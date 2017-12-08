# Motivation
 We want to find out if humans have discovered yet that lab rats and dolphins are smarter than them so our question is: who’s the smartest animal in town? 

* __The dataset__
The posts from 3 Facebook groups:

* Animal Cognition - 6 956 posts

* Animal Cognition, the Emotional and Intellectual Lives of Animals - 10 364 posts

* Anthrozoology - 7 442 posts

* 24 762 posts in total, 78.3 MB of pickles


* __Choice of dataset__
We decided that these were the 3 most relevant Groups: Animal Cognition, Animal Emotional Lives, Anthrozoology. Since these facebook groups are all about science, more specifically the intelligence of animals, our assumption is that if a post on these groups mentions an animal, that animal must be smart.

* __Goal for the end user's experience__
>

# Basic stats about the dataset


Each downloaded post initially contains:

* reactions
* attachments
* shares
* created_time
* message
* story
* from
* comments

       * reactions
       * from
       * comments
       * created_time
       * message
       * id
* story_tags
* type
* description
* link
* name
* sharedposts
* updated_time
* caption

Upon cleaning and preprocessing, we added some other 'fields' to each post:
* __animals_detected__: animals which were mentioned in the post, detected with RegEx, from a list of all animals from Wikipedia
* __text_tokens__: all the tokenized text from description, comments, message, caption
* __animals_subject__: the animal that the post is about
* __sentiment__: the sentiment of the post
* __text_tokens_stemmed__: stems of all the words in the post's text
* __date_time__: the date and time when the post was created, converted in _datetime_ format

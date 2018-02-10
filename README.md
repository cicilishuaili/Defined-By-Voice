# Defined-By-Voice

## Motivation
Language is powerful, and not only in the ways we use it for communication and expression. Studies have shown that the medium with which we share our thoughts, ideas, beliefs in, inadvertently influences and shapes us. From [national identity](https://www.npr.org/sections/parallels/2017/09/29/554327011/for-catalonias-separatists-language-is-the-key-to-identity), to [our spending habits](http://www.anderson.ucla.edu/faculty/keith.chen/papers/LanguageWorkingPaper.pdf), to perceptions of [time](http://journals.sagepub.com/doi/abs/10.1177/0956797610386621), [agency](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00162/full), and [art](https://www.frontiersin.org/articles/10.3389/fpsyg.2010.00244/full), the features of language matter more than you may think. As a speaker of two languagages without grammatical gender, I found it especially interesting the way that can affect [how inanimate objects are described](https://web.stanford.edu/class/linguist156/Boroditsky_ea_2003.pdf), showing just how stereotypes can be ingrained and propagated via language.

As technology advances rapidly, it acts as a mirror of these [embedded biases](http://science.sciencemag.org/content/356/6334/183). Despite being supposedly genderless, like "cacti and certain species of fish", voice assistants in our phones, speakers and computers sound [overwhelmingly female](https://www.wsj.com/articles/alexa-siri-cortana-the-problem-with-all-female-digital-assistants-1487709068). 

Fascinated by the ways voices are embedded in our lives, I aim to poke and probe at the intersection of language and gender.
Originally I intended the project on being centered around the example sentences given by various online dictionaries to detect implicit sexism. But given that many dictionaries take their sources for such examples usage from various corporas, the conclusion is likely forgone. Oxford Dictionary, for one, has already been [criticized for their cited usage](https://www.theguardian.com/books/2016/jan/25/oxford-dictionary-review-sexist-language-rabid-feminist-gender) of adjectives including "rabbid", "nagging", "shrill", and "grating".

## Problem
This current project aims to process and categorize audio clips of word pronunciations from online libraries that have multiple voices of different genders in attempt to answer the question: are gendered/stereotypically gendered words more likely to be voiced by that gender?

## Data Source
Suitable candidates found for online dictionaries include but are not limited to Merriam Webster, dictionary.com, Oxford dictionary, Cambridge dictionary, and McMilland dictionary. Google's dictionary audio files unfortunately does not allow for crawling as specified in their robots.txt.

## Analysis
The basic plan of approach thus far:

1. Scrape online dictionaries for audio files
2. Process the files and extract relevant features
3. Classify voice as that of a male or female

To this end, Kaggle has a good starting point for [predicting gender based on voice] (https://www.kaggle.com/primaryobjects/voicegender) which will likely be of great utility to start.

Separately, the task of "gendered words" can be tackled via various means:

* Vectorize the words and quantify bias by distance from "he"/"she" algorithmically; collocation frequencies of words with "he"/"she"
* Use words that are perceived categorically skewed as one gender in studies (e.g. http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.464.8919&rep=rep1&type=pdf)
* Use words that imply gender (e.g. king/queen, aunt/uncle, bachlor/bachlorette, mare/colt)

I look forward to learning various useful tools concerning classification, NLP, large scale processing of various forms of digit media. The project can be event extended to other languages if suitable data sources are found, and may prove easier since many languages have grammatical gender, naturally lending itself to a gender category. Ultimately we can give a particular dictionary a grade on gender neutrality.

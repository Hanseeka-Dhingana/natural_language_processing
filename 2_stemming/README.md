The modern English language is considered a weakly inflected language. This means there are many words in English derived from another word; for example, the inflected word “normality” is derived from the word “norm,” which is the root form. All inflected languages consist of words with common root forms, but the degree of inflection varies based on the language. 

When working with text, sometimes it’s necessary to apply normalization techniques to get words to their root form from their derived versions. This helps reduce randomness and bring the words in the corpus closer to the predefined standard, improving the processing efficiency since the computer has fewer features to deal with. 

Two popular text normalization techniques in the field of Natural Language Processing (NLP), the application of computational techniques to analyze and synthesize natural language and speech, are **stemming and lemmatization.**    

## Stemming  
Stemming is a technique used to reduce an inflected word down to its word stem. For example, the words “programming,” “programmer,” and “programs” can all be reduced down to the common word stem “program.” In other words, “program” can be used as a synonym for the prior three inflection words.   

Stemming algorithms function by taking a list of frequent `prefixes` and `suffixes` found in inflected words and chopping off the end or beginning of the word. This can occasionally result in word stems that are not real words; thus, we can affirm this approach certainly has its pros, but it’s not without its limitations.     

### Advantages of Stemming    
- **Improved model performance**: Stemming reduces the number of unique words that need to be processed by an algorithm, which can improve its performance. Additionally, it can also make the algorithm run faster and more efficiently.    

- **Grouping similar words:** Words with a similar meaning can be grouped together, even if they have distinct forms. This can be a useful technique in tasks such as `document classification,` where it’s important to identify key topics or themes within a document.   

- **Easier to analyze and understand:** Since stemming typically reduces the size of the vocabulary, it’s much easier to analyze, compare, and understand texts. This is helpful in tasks such as `sentiment analysis,` where the goal is to determine the sentiment of a document.    

### Disadvantages of Stemming    

- **Overstemming (False Positives):** Unrelated words are incorrectly reduced to the same stem (e.g., universe, university, universal), leading to reduced accuracy in tasks like search or classification.

- **Understemming (False Negatives):** Related words are not reduced to the same stem (e.g., alumnus, alumnae, alumni), missing meaningful connections.

- **Language Complexity:** Stemmers are harder to build for morphologically rich languages (like Italian or Russian), due to complex inflections and grammar rules.
 

## Lemmatization 
Lemmatization is another technique used to reduce inflected words to their root word. It describes the algorithmic process of identifying an inflected word’s “lemma” (dictionary form) based on its intended meaning. 

As opposed to stemming, lemmatization relies on accurately determining the intended part-of-speech and the meaning of a word based on its context. `For example,` you can expect a lemmatization algorithm to map “runs,” “running,” and “ran” to the lemma, “run.” 

### Advantages of Lemmatization
- **Accuracy:** Lemmatization does not merely cut words off as you see in stemming algorithms. Analysis of words is conducted based on the word’s POS to take context into consideration when producing lemmas. Also, lemmatization leads to real dictionary words being produced.
### Disadvantages of Lemmatization 
- **Time-consuming:** Compared to stemming, lemmatization is a slow and time-consuming process. This is because lemmatization involves performing morphological analysis and deriving the meaning of words from a dictionary. 


## Question: “should I use stemming or lemmatization for text preprocessing?” 

- Do you care about speed and efficiency? If so, choose stemming. 
- Is context important for your application? If you said “yes,” then use lemmatization. 
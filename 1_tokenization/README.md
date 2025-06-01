# Tokenization
Tokenization, in the realm of Natural Language Processing (NLP) and machine learning, refers to the process of converting a sequence of text into smaller parts, known as tokens. These tokens can be as small as characters or as long as words. The primary reason this process matters is that it helps machines understand human language by breaking it down into bite-sized pieces, which are easier to analyze.   

The primary goal of tokenization is to represent text in a manner that's meaningful for machines without losing its context. By converting text into tokens, algorithms can more easily identify patterns. This pattern recognition is crucial because it makes it possible for machines to understand and respond to human input. For instance, when a machine encounters the word "running", it doesn't see it as a singular entity but rather as a combination of tokens that it can analyze and derive meaning from.

**Example**
To delve deeper into the mechanics, consider the sentence, **"Chatbots are helpful."** When we tokenize this sentence by words, it transforms into an array of individual words:

`["Chatbots", "are", "helpful"].`

This is a straightforward approach where spaces typically dictate the boundaries of tokens. However, if we were to tokenize by characters, the sentence would fragment into:

`["C", "h", "a", "t", "b", "o", "t", "s", " ", "a", "r", "e", " ", "h", "e", "l", "p", "f", "u", "l"].`

This character-level breakdown is more granular and can be especially useful for certain languages or specific NLP tasks.   

![alt text](/assets/token.png)  

## Types of Tokenization 
|Types |Description | Use Cases|
|-------------------|----------------------------------|--------------------------------------------------------------------|
|Word Tokenization	|Breaks text into individual words.|	Effective for languages with clear word boundaries like English.|
|Character Tokenization|	Segments text into individual characters.	|Useful for languages without clear word boundaries or tasks requiring granular analysis.|
|Subword Tokenization	|Breaks text into units larger than characters but smaller than words.	|Beneficial for languages with complex morphology or handling out-of-vocabulary words.|

## Tokenization Use Cases

Tokenization serves as the backbone for a myriad of applications in the digital realm, enabling machines to process and understand vast amounts of text data.   

- Search engines
- Machine translation
- Speech recognition
- Sentiment analysis in reviews
- Chatbots and virtul assistants

## Tokenization Challanges 
Tokenization sounds simple splitting text into smaller parts, but human language is messy and complex, which makes it tricky.   

**1) Ambiguity**  
The same sentence can have more than one meaning, depending on how it's understood or tokenized.  

**Example**   "Flying planes can be dangerous."

Meaning 1: Piloting planes is risky.
- "Flying" = verb (action)

Meaning 2: Planes that are flying can be dangerous.
-  "Flying" = adjective (describes the planes)   

**2) Languages without clear boundaries**  
Some languages (like Chinese, Japanese, Thai) don’t use spaces between words, so it's difficult to know where one word ends and another begins.

**Example** (Chinese):
Sentence: 我喜欢吃苹果
(Human translation: "I like to eat apples")

But without spaces, it looks like:
**我喜 欢吃 苹 果**
Should it be:

- 我 / 喜欢 / 吃 / 苹果 
or

- 我 / 喜 / 欢吃 / 苹 / 果 

**How to solve this** 
Advanced multilingual models like:

- **XLM-R (Cross-lingual RoBERTa)**
- **mBERT (Multilingual BERT)**

Use subword tokenization and are trained on many languages, so they learn how words are formed, even in languages with no spaces.

They tokenize text like this:
``` 
  "喜欢吃苹果" → ["喜", "欢", "吃", "苹果"]
```   
OR  
``` 
    ["喜", "##欢", "吃", "苹", "##果"]
```
The `##` means it’s a continuation of the previous subword (WordPiece/BPE style).  


**3) Handling Special Characters**  
Emails, URLs, hashtags, and code-like text are tricky should we split them or keep them together?  

**Example**   "john.doe@email.com"

Should it be tokenized as:
- ["john.doe@email.com"] (one token)?  
OR
- ["john", ".", "doe", "@", "email", ".", "com"] (many tokens)?
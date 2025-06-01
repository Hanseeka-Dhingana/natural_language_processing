# NLP (Natural Language Processing)  
Natural language processing (NLP) is a subfield of computer science and artificial intelligence (AI) that uses machine learning to enable computers to understand and communicate with human language.  

NLP involves enabling machines to understand, interpret, and produce human language in a way that is both valuable and meaningful. OpenAI, known for developing advanced language models like ChatGPT, highlights the importance of NLP in creating intelligent systems that can understand, respond to, and generate text, making technology more user-friendly and accessible.  

## How Does NLP Work?
Let’s take a look at some of the mechanisms at work behind natural language processing.

### Components of NLP
Natural Language Processing is not a monolithic, singular approach, but rather, it is composed of several components, each contributing to the overall understanding of language. The main components that NLP strives to understand are Syntax, Semantics, Pragmatics, and Discourse.

#### Syntax   
- **Definition:** Syntax pertains to the arrangement of words and phrases to create well-structured sentences in a language.   
- **Example:** Consider the sentence "The cat sat on the mat." Syntax involves analyzing the grammatical structure of this sentence, ensuring that it adheres to the grammatical rules of English, such as subject-verb agreement and proper word order
#### Semantics
- **Definition:** Semantics is concerned with understanding the meaning of words and how they create meaning when combined in sentences.
- **Example:** In the sentence "The panda eats shoots and leaves," semantics helps distinguish whether the panda eats plants (shoots and leaves) or is involved in a violent act (shoots) and then departs (leaves), based on the meaning of the words and the context.
#### Pragmatics
- **Definition:** Pragmatics deals with understanding language in various contexts, ensuring that the intended meaning is derived based on the situation, speaker’s intent, and shared knowledge.
- **Example:** If someone says, "Can you pass the salt?" Pragmatics involves understanding that this is a request rather than a question about one's ability to pass the salt, interpreting the speaker’s intent based on the dining context.
#### Discourse
- **Definition:** Discourse focuses on the analysis and interpretation of language beyond the sentence level, considering how sentences relate to each other in texts and conversations.
- **Example:** In a conversation where one person says, "I’m freezing," and another responds, "I’ll close the window," discourse involves understanding the coherence between the two statements, recognizing that the second statement is a response to the implied request in the first.

### NLP techniques and methods
To analyze and understand human language, NLP employs a variety of techniques and methods. Here are some fundamental techniques used in NLP:

- [**Tokenization**](1_tokenization). This is the process of breaking text into words, phrases, symbols, or other meaningful elements, known as tokens.
- **Parsing**. Parsing involves analyzing the grammatical structure of a sentence to extract meaning.
- [**Lemmatization.**](2_stemming) This technique reduces words to their base or root form, allowing for the grouping of different forms of the same word.
- **Named Entity Recognition (NER)**. NER is used to identify entities such as persons, organizations, locations, and other named items in the text.
- **Sentiment analysis**. This method is used to gain an understanding of the sentiment or emotion conveyed in a piece of text.    


## Real World Application
- Contextual Advertisements
- Email Clients - Spam filtering, smart reply 
- Social Media - removing adult content, opinion mining 
- Search Engines 
- Chatbots


## Common NLP Tasks
- Text/Document Classification
- Sentiment Analysis
- Information Retrieval
- Parts of Speech Tagging 
- Language Detection and Machine Translation 
- Conversational Agents 
- Knowledge Graph and QA systems 
- Text Summarization
- Topic Modelling 
- Text Generation
- Spell Checking And Grammar Correction 
- Text Parsing 
- Speech To Text 


## Aproaches to NLP  
- Heuristic Approaches 
    - Regular Expression
    - Wordnet
    - Open Mind Common Sense

- Machine Learning 
    - Navie Bayes
    - Logistic Regression
    - SVM
    - LDA 
    - Hidden Markov Model

- Deep Learning Approach
    - RNN (sequential data)
    - LSTM (memory factor is better than RNN)
    - GRU/CNN
    - Transformers
    - Autoencoder 



## Challenges in NLP 
**1) Ambiguity** 
Sentences have more than one meaning. It is difficult for machine to understand the right meaning.   

Example: 
- I saw the boy on the beach with my binoculars.  
- I have never tastes a cake quite like that one before!  

**2) Contextual Words** 
Same words have more than one meaning according to the context.  

Example: I `ran` to the store because we `ran` out of milk.

**3) Collaquialisms and slang**  
**Collaquialisms:** Informal words or phrases used in everyday conversation, often specific to a region or culture.

Example:   "Gonna" (going to), "y'all" (you all), "wanna" (want to)

**Slang :** Very informal or trendy words often used by specific groups, and which may change over time.	

Example:  "Lit" (exciting), "Ghosted" (suddenly stop communicating), "Cap" (lie)

**4) Synonyms** 
**5) Irony, Sarcasm and tonal diff** 
**6) Spelling Errors** 
**7) Creativity** 
**8) Diversity** 


## End to End NLP Pipeline 
NLP software consists of the following steps: 
- Data Acquisition 
- Text Preparation 
   - Text Cleanup
   - Basic Preprocessing
   - Advance Preprocessing

- Feature Engineering 
- Modeling 
   - Model Building
   - Evaluation

- Deployment
   - Deployment
   - Monitoring
   - Model Updated
# Named Entity Recognition (NER)  
NER is the bridge between the unstructured data and structured data.   

NER's primary objective is to comb through unstructured text and identify specific chunks as named entities, subsequently classifying them into predefined categories. This conversion of raw text into structured information makes data more actionable, facilitating tasks like data analysis, information retrieval, and knowledge graph construction.

## How it work
The intricacies of NER can be broken down into several steps:

- **Tokenization.** Before identifying entities, the text is split into tokens, which can be words, phrases, or even sentences. For instance, "Steve Jobs co-founded Apple" would be split into tokens like "Steve", "Jobs", "co-founded", "Apple".
- **Entity identification.** Using various linguistic rules or statistical methods, potential named entities are detected. This involves recognizing patterns, such as capitalization in names ("Steve Jobs") or specific formats (like dates).
- **Entity classification.** Once entities are identified, they are categorized into predefined classes such as "Person", "Organization", or "Location". This is often achieved using machine learning models trained on labeled datasets. For our example, "Steve Jobs" would be classified as a "Person" and "Apple" as an "Organization".
- **Contextual analysis.** NER systems often consider the surrounding context to improve accuracy. For instance, in the sentence "Apple released a new iPhone", the context helps the system recognize "Apple" as an organization rather than a fruit.
- **Post-processing.** After initial recognition and classification, post-processing might be applied to refine results. This could involve resolving ambiguities, merging multi-token entities, or using knowledge bases to enhance entity data.  

## Applications of NER (Named Entity Recognition)

1. **News Aggregation**:
   Helps categorize news articles by people, places, or organizations, making it easier for readers to find relevant stories.

2. **Customer Support**:
   Speeds up analysis of customer queries by identifying product/service-related issues for quicker resolution.

3. **Research**:
   Assists researchers in scanning large texts to find key entities, streamlining data analysis and saving time.

4. **Legal Document Analysis**:
   Automates the identification of names, dates, and locations in legal texts, enhancing research efficiency.

## Challenges in Named Entity Recognition (NER)

1. **Ambiguity**:
   Same word may refer to different entities (e.g., *Amazon* as a company or a river).

2. **Context Dependency**:
   Meaning of entities depends heavily on surrounding text (e.g., *Apple* as fruit vs. tech company).

3. **Language Variations**:
   Slang, dialects, and regional expressions make entity recognition complex.

4. **Data Sparsity**:
   Lack of labeled data, especially in rare languages or domains, limits model performance.

5. **Model Generalization**:
   Models trained in one domain may not perform well in others, affecting scalability.

## Step to using NER  
- Importing necessary packages 
- Loading the Data and NER model 
- Entity Ruler 
- Clean the Text
- Entity Recognition 
- Match Score 


# Text-Summarization-using-NLTK

### Objective:
This project aims to automatically generate a concise summary of a given text using Natural Language Processing (NLP) techniques. The implementation is done using the NLTK (Natural Language Toolkit) library in Python.

### Key Features & Methodology:
1️. Preprocessing the Text

 - Removes extra spaces and punctuation using Regular Expressions (re).
    
 - Tokenizes the text into sentences using sent_tokenize().

 - Tokenizes sentences into words using word_tokenize().

 - Converts all words to lowercase for uniformity.

2️. Removing Stopwords

 - Common words like "is", "the", "and", etc., are removed using NLTK's stopwords list to focus on meaningful words.

3. Computing Word Frequencies

  - Each word's occurrence is counted.

 - Frequencies are normalized by dividing by the most frequent word’s count (for scaling between 0 and 1).

4. Scoring Sentences

  - Each sentence is scored based on the sum of its word frequencies.
 
  - Higher scores indicate more important sentences.

5. Extracting the Summary

   - Uses heapq.nlargest() to select the top N most important sentences.

   - Joins the selected sentences to form a meaningful summary.

### Technologies Used:
✅ Python – Programming language

✅ NLTK – Tokenization, stopword removal, and processing

✅ Regular Expressions (re) – Text cleaning

✅ Heapq – Selecting top sentences efficiently


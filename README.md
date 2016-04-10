#Stock Forecasting   
Using simple dicitonary-based sentiment analysis, this script looks to predict what near-future stock prices will
be for a specific company based on their aggregate sentiment scores. 
  
Sentiment will be gathered from the following sources:  
	
*Twitter  
*The Huffington Post  
*More sources will be added as more code is written

##Methodology  

For now, the methodology of determining sentiment is extremely simple. Rather than using a Naive Bayes "bag of words" 
model, a sentiment lexicon is going to be used. There are two levels of sentiment given for each word, 
"weak and strong". While there are classifications for things outside of "negative" and "positive", this study will 
only use those two for measuring the strength and polarity of the sentiment. 
  
The sentiment will be determined using the following steps:  
  
1. Tokenize the body of the article/tweet  
2. Match it with the same word in the sentiment lexicon  
3. Multiply the polarity (either Positive or Negative, represented as +1 or -1) by the strength of the sentiment (either .5 or 1, depending on if it has 'weak' or 'strong' sentiment)
4. Divide that number by the number of tokens in the body of the paragraph  

###Model/Algorithm Methodology will be added at a later date, once it has been implemented

##Tools/Libs Used  
This code is written in Python and relies heavily on the Pandas library.

###For now there is no way to run all scripts at once, each one must be run individually and in order. This will be fixed with a coming update, as is having to manually enter the company name and symbol

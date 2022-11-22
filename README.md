## 1.1 What is NLP?  

Let’s get to know what Natural Language Processing is. Right now, as we are reading and writing this report,
we our brain is actually forming some sort of comprehension from it. When we program a computer do it, it is 
known as Natural Language Processing. Natural Language Processing is a very useful in all sorts of textual 
based AI applications. NLP starts with unstructured text, which is how we speak and interpret text. For example, 
some unstructured text is "add cheese and bread to my grocery list." Now we understand exactly what that 
means, but it is unstructured to a computer. So, what we proceed to do, is to create a structured representation of 
that same information that a computer can process. Now list of groceries can be considered as a big list and then 
it has elements within it, like cheese, and bread. Now this is a structured list. The job of natural language 
processing is to translate between unstructured and structured data sitting right in the middle.

Natural Language Processing is used in various Machine Learning and Artificial Intelligence applications to 
derive insights from textual data. Corporations, scientists, and governments use it across the world to understand 
user behaviour, sentiments, opinion and much more. Let’s go through the tasks that can be accomplished by 
Natural Language Processing. These include language translation, similar sentence identification, paragraph 
summarization, text classification (e.g., spam message filtering), sentiment analysis (e.g., Positive, Neutral or 
Negative user feeling), question answering, conversational agents and chatbots.

## 1.2 Bag of Words  

As we have seen earlier computers can’t understand language like we do. Computers understand numbers, more 
specifically into vectors. Bag of words is one of the ways to achieve this. So basically, bag of words is way to 
represent some text mathematically for modelling a machine learning algorithm. It’s based on the concept 
that if two sentences have matching words then they are similar. Bag of words is modelled after 2 things.
  1. Generate a vocabulary of all the words and characters in the entire corpus of given sentences.
  2. Measure which words are present in which sentences by creating a vector.  
  
Bag of words is usually combined with techniques of Lemmatisation or stemming after removing stop words 
from the sentences to get final vector representation. The downside of this technique is that it does not take into 
regard into order or structure which could reveal more meaningful information about the sentences.  

## 1.3 Stemming  

Words in any language originate from a main word, these are referred as Stem words and derivative words 
branch out of this stem. These branched words mean the same but have different forms depending upon the 
grammar of the sentences. Now we want these branched words to be reduced to their corresponding stem words.
Stemming in Natural Language Processing does exactly this, reduces words to their stem words. For example,
let’s consider the word ‘stem’ itself. This can take forms such as ‘stemming’ or ‘stemmed’. So, the words 
‘stemming’ or ‘stemmed’ have to be reduced to ‘stem’.  

## 1.4 Lemmatization  

Lemmatization is very similar to stemming. It also reduces the words to their root stem, but there is a catch.
Stemming usually reduces words to a form where they lose their meaning. Lemmatization overcomes this by 
keeping this to the minimum. However, this technique sometimes can lead to some same stem words not to be 
detected efficiently. But it works well compared to stemming from a word understanding point of view. This is 
evident from the above figure. The word ‘Histori’ does not ring a bell instantly. After lemmatisation the word 
‘historical’ is kept as it is. This helps in creating a more meaningful corpus, thus is very useful, since the parts 
of speech are preserved. Lemmatization’s limitations are overcome by word to vector embedding.  

## 1.5 Word to Vector and Word Embedding  

As we have seen what Bag of Words, Stemming and Lemmatization do and how they work an important 
drawback is observed, i.e., they don’t preserve semantic information. What this means is that the relationship 
between the words is not known. Let’s take a simple example, suppose we have three words ‘man’, ‘woman’ 
and ‘play’. Immediately we human can perceive that ‘man’ and ‘woman’ are almost similar in the sense both 
refer to human but different genders that all. Now we need to make computers understand this. This is where the 
word to vector comes.  

In this model each word is represented as vector of multiple dimensions (32 or more). This vector representation 
is called word embedding and depends on what kind of model we are using (such as Word2vec, GloVe or BERT 
embeddings). Thus, semantic information is preserved in this way. Also, computers can build a graph internally 
which can be used to traverse to understanding semantics. Let’s outline the steps to create a word to vector 
representation:
  1. Tokenize the sentences to convert them into word tokens
  2. Create a histogram of the tokens obtained
  3. Then create a matrix of all the unique tokens and represent the occurrence and relationship between the
words and nearby words that lead to it by cosine similarity


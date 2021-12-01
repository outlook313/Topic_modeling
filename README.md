# Topic_modeling
Term Frequency – Inverse Document Frequency (TF-IDF)<br>
Latent Semantic Analysis (LSA)


<b>Topic Modeling:</b><br><br>
Within NLU, which is a part of NLP, one of the many tasks that can be performed is
extracting the meaning of a sentence, a paragraph, or a whole document. One approach
to understanding a document is through its topics. For example, if a set of documents
is from a newspaper, the topics might be politics or sports. With topic modeling
techniques, we can obtain a bunch of words representing various topics. Depending
on your set of documents, you will then have different topics represented by different
words. The goal of these techniques is to know the different types of documents in your
corpus.
  
![topic_modeling](https://user-images.githubusercontent.com/89722385/144175229-948abb02-2382-498b-a029-e650fc67e20e.jpeg)

<b>1.Term Frequency – Inverse Document Frequency (TF-IDF):</b><br><br>
TF-IDF is a commonly used NLP model for extracting the most important words from
a document. To perform this classification, the algorithm will assign a weight to each
word. The idea of this method is to ignore words without relevance to the meaning of a
global concept, (which means the overall topic of a text), so those terms will be down-
weighted (which means that they will be ignored). Down-weighing them will allow us to
find the keywords of that document (the words with the greatest weights).
Mathematically, the algorithm to find the weight of a term in a document is as follows:
  
  
                        W i,j=  t f i,j *log(N/d fi)
  
  * W i,j :Weight of the term ,i ,in the decument, j.<br>
  * tf,j :Number of Occurences of i in j.<br>
  * df,j :Number of documents containing i.<br>
  * N :Total number of Documents.<br><br>
  
The result is the number of times a term appears in that document, multiplied by the
log of the total number of documents, divided by the number of documents that contain
the term.

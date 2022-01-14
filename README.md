# Text Readability Classifier

Research into the area of text readability has become increasingly important over the past few years, given how much data is produced online on a daily basis.
Writers are expected to produce original written thought, or “copy” within a specified word count due to space constraints and low attention spans (Goldhaber,
1997), which makes it increasingly important to make sure that the compact texts still reaches a wide range of audience and are easy to understand. Even teachers, while creating a reading list for students, might make use of a text readability software to ensure that they’re choosing books that are in tandem with their students’ reading level, as the student pool could comprise of children with learning disabilities, immigrant populations, and second or foreign language learners (Vajjala and Meurers, 2012). As a result, a consistent and reliable method for determining if a text is accessible to the target population is required.

Aim: To construct a model that allows writers to have more control over their writing, so that they could structure their work according to their intended audience.
 
The purpose of this project was to build and analyse various deep learning models for text readability classification in order to determine whether a piece of text is easy or hard to read. Naive Bayes, Convolutional Neural Network, and distilBERT were trained on self-built labelled corpora. The reason for choosing only two labels (easy or hard) was to avoid multi-label classification in order to make the task for the classifier simpler. The dataset was also analysed using word
embeddings with t-SNE. Lastly, upon all the classifiers being ready, they were tested using Wiki-Simple and Wiki-Normal pages. A thorough analysis of all the
findings have been included in the supporting project essay here [link]. 

Corpus Development:

English textbooks from India, Afghanistan, Indonesia, and the Islamic State were interchangeably used to form three separate datasets. This was done for several
different aims: to see if variances in grade ranges affect the performance, to study how the same language is taught in different regions, to see if changes in
region of the textbook utilized for the same classifier affected performance, and to verify if the model could accurately classify English phrases from across
the world using non-western data. Due to this data diversity, one can evaluate what effects the specifics of each dataset have on the general robustness of the
classifier. The nature of the content was common in all the textbooks, consisting of stories, poems, plays, and english language acquisition exercises. All of
these texts were sourced from Library Genesis (Library Genesis, 2021) and extracted from PDF files using an online file converter. The three finalised datasets
with labels were as follows:
 
a)	Dataset 1: First and Tenth Grade English Textbooks from India by the National Council of Educational Research and Training Publication (2009 Edition) 

b)	Dataset 2: Fourth and Twelfth Grade English Textbooks from Afghanistan by the country's Ministry of Education (2011 Edition)

c)	Dataset 3: A Second Grade English Textbook from Indonesia and a Sixth Grade Textbook from the Islamic State.





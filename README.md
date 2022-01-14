# Text Readability Classifier

Research into the area of text readability has become increasingly important over the past few years, given how much data is produced online on a daily basis.
Writers are expected to produce original written thought, or “copy” within a specified word count due to space constraints and low attention spans (Goldhaber,
1997), which makes it increasingly important to make sure that the compact texts still reaches a wide range of audience and are easy to understand. Even teachers,
while creating a reading list for students, might make use of a text readability software to ensure that they’re choosing books that are in tandem with their
students’ reading level, as the student pool could comprise of children with learning disabilities, immigrant populations, and second or foreign language learners
(Vajjala and Meurers, 2012). As a result, a consistent and reliable method for determining if a text is accessible to the target population is required.

Aim: To construct a model that allows writers to have more control over their writing, so that they could structure their work according to their intended audience.
 
The purpose of this project was to build and analyse various deep learning models for text readability classification in order to determine whether a piece of text
is easy or hard to read. Naive Bayes, Convolutional Neural Network, and distilBERT were trained on self-built labelled corpora. The reason for choosing only two
labels (easy or hard) was to avoid multi-label classification in order to make the task for the classifier simpler. The dataset was also analysed using word
embeddings with t-SNE. Lastly, upon all the classifiers being ready, they were tested using Wiki-Simple and Wiki-Normal pages. A thorough analysis of all the findings have been included in the supporting project essay here [link]. 






# Text Readability Classifier

`This was my project for the unit 'Natural Language Processing for the Creative Industries' at the University of the Arts London during Term 1 of my masters program.`

Research into the area of text readability has become increasingly important over the past few years, given how much data is produced online on a daily basis.
Writers are expected to produce original written thought, or “copy”, within a specified word count due to space constraints and low attention spans (Goldhaber,
1997), which makes it increasingly important to make sure that these compact texts still reaches a wide range of audience, and that they are easy to understand.
Even teachers, while creating a reading list for students, might make use of a text readability software to ensure that they’re choosing books that are in tandem
with their students’ reading level, as the student pool could comprise of children with learning disabilities, immigrant populations, and second or foreign
language learners (Vajjala and Meurers, 2012). As a result, a consistent and reliable method for determining if a text is accessible to the target population is
required.

**Aim: To construct a model that allows writers to have more control over their writing, so that they could structure their work according to their intended
audience.**
 
The purpose of this project was to build and analyse various deep learning models for text readability classification in order to determine whether a piece of
text is easy or hard to read. Naive Bayes, Convolutional Neural Network, and distilBERT models were trained on a self-curated corpus which was divided into
three distinct labelled datasets. Each of these datasets were also analysed using word embeddings with t-SNE to get a better understanding of it. Lastly, upon
all the classifiers being ready after manual parameter-tweaking, they were tested using Wiki-Simple and Wiki-Normal pages. 

### Corpus Development:

English textbooks from India, Afghanistan, Indonesia, and the Islamic State were interchangeably used to form three separate datasets. This was done for several
different aims: to see if variances in grade ranges affect the performance, to study how the same language is taught in different regions, to examine if changes
in region of the textbook utilized for the same classifier affected performance, and to verify if the model could accurately classify English phrases from across
the world using non-western data. Due to this data diversity, one can evaluate what effects the specifics of each dataset has on the general robustness of the
classifier. The nature of the content was common in all the textbooks, consisting of stories, poems, plays, and english language acquisition exercises. All of
these texts were sourced from Library Genesis, and extracted from PDF files using an online file converter. The three finalised datasets
with labels were as follows:
 
a)	Dataset 1: [First and Tenth Grade English Textbooks from India](https://libgen.is/search.php?req=ncert+english&open=0&res=25&view=simple&phrase=1&column=def) by the country's National Council of Educational Research and Training Publication (2009 Edition)

b)	Dataset 2: [Fourth and Twelfth Grade English Textbooks from Afghanistan](https://libgen.is/search.php?req=afghanistan+english&lg_topic=libgen&open=0&view=simple&res=25&phrase=1&column=def) by the country's Ministry of Education (2011 Edition)

c) Dataset 3: A [Second Grade English Textbook from Indonesia](https://libgen.is/book/index.php?md5=42EEC448F886A2790FC9AE5A2526F0C4) by the country's Ministry of Education and Culture (2008 Edition), and a [Sixth Grade Textbook from the Islamic State](https://libgen.is/search.php?req=islamic+state+english&open=0&res=25&view=simple&phrase=1&column=def) (Publisher unknown).


**A thorough analysis of all the findings have been included in the supporting critical essay [here.](https://github.com/ashwathi-pillai/text-readability-classifier/blob/main/critical%20essay.pdf)** 


### REFERENCES: 

1) Bormuth, J., 1966. Readability: A New Approach. Reading Research Quarterly, [online] 1(3), pp.3-8. Available at: <https://www.jstor.org/stable/747021?seq=1#metadata_info_tab_contents> [Accessed 14 December 2021].

2) Brownlee, J., 2021. Overfitting and Underfitting With Machine Learning Algorithms. [online] Machine Learning Mastery. Available at: <https://machinelearningmastery.com/overfitting-and-underfitting-with-machine-learning-algorithms/> [Accessed 17 December 2021].

3) Chah, N., 2021. Apply word2vec to all sorts of text documents.. [online] GitHub. Available at: <https://github.com/nchah/word2vec4everything> [Accessed 14 December 2021].

4) Code.Google.com, 2021. Word2Vec - Google Code. [online] Code.Google.com Available at: <https://code.google.com/archive/p/word2vec/> [Accessed 17 December 2021].

5) Olms.cte.jhu.edu, 2021. Cloze Procedure : Student Compass: Instructional Strategies Bank. [online] Available at: <http://olms.cte.jhu.edu/olms2/7243> [Accessed 17 December 2021].

6) Delaney, J., 2021. Visualizing Word Vectors with t-SNE. [online] Kaggle.com. Available at: <https://www.kaggle.com/jeffd23/visualizing-word-vectors-with-t-sne> [Accessed 16 December 2021].

7) Goldhaber, M., 1997. The attention economy and the Net. First Monday, [online] Available at: <https://firstmonday.org/article/view/519/440> [Accessed 13 December 2021].

8) Horton, R., 1974. The Construct Validity of Cloze Procedure: An Exploratory Factor Analysis of Cloze, Paragraph Reading, and Structure-of-Intellect Tests. Reading Research Quarterly, [online] 10(2), p.248. Available at: <https://www.jstor.org/stable/pdf/747185.pdf?refreqid=excelsior%3Acf937d464f35e0adfc10d11b7b1496f3> [Accessed 6 December 2021].

9) Kincaid, J., Fishburne, R., Rogers, R. and Chissom, B., 1975. Derivation Of New Readability Formulas (Automated Readability Index, Fog Count And Flesch Reading Ease Formula) For Navy Enlisted Personnel. [online] Available at: <https://stars.library.ucf.edu/cgi/viewcontent.cgi?article=1055&context=istlibrary> [Accessed 15 December 2021].

10) Klare, G., 2000. The measurement of readability. ACM Journal of Computer Documentation, [online] 24(3), pp.107-121. Available at: <https://dl.acm.org/doi/pdf/10.1145/344599.344630> [Accessed 5 December 2021].

11) Maheshwari, A., 2021. Report on Text Classification using CNN, RNN & HAN. [online] Medium. Available at: <https://medium.com/jatana/report-on-text-classification-using-cnn-rnn-han-f0e887214d5f> [Accessed 17 December 2021].

12) Martinc, M., Pollak, S. and Robnik-Šikonja, M., 2019. Supervised and Unsupervised Neural Approaches to Text Readability. Computational Linguistics, [online] 47(1), pp.141-179. Available at: <https://direct.mit.edu/coli/article/47/1/141/97334/Supervised-and-Unsupervised-Neural-Approaches-to> [Accessed 16 December 2021].

13) McAuliffe, D., 2021. Developments in AI: Language models - Arabesque. [online] Arabesque. Available at: <https://www.arabesque.com/2021/07/06/developments-in-ai-language-models/> [Accessed 17 December 2021].

14) Pogiatzis, A., 2021. NLP: Contextualized word embeddings from BERT. [online] Medium. Available at: <https://towardsdatascience.com/nlp-extract-contextualized-word-embeddings-from-bert-keras-tf-67ef29f60a7b> [Accessed 17 December 2021].

15) Ray, S., 2021. Learn Naive Bayes Algorithm | Naive Bayes Classifier Examples. [online] Analytics Vidhya. Available at: <https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/> [Accessed 16 December 2021].

16) Sanh, V., Debut, L., Chaumond, J. and Wolf, T., 2019. DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter. [online] Available at: <https://arxiv.org/pdf/1910.01108v4.pdf> [Accessed 17 December 2021].

17) Schriver, K., 2017. Plain Language in the US Gains Momentum: 1940–2015. IEEE Transactions on Professional Communication, [online] 60(4), pp.343-383. Available at: <https://www.plainlanguage.gov/media/Schriver%20Plain%20Language%20in%20US%20Gains%20Momentum%201940_2015%20Draft.pdf> [Accessed 12 December 2021].

18) Vajjala, S. and Meurers, D., 2012. On Improving the Accuracy of Readability Classification using Insights from Second Language Acquisition. [online] pp.163-165. Available at: <https://dl.acm.org/doi/pdf/10.5555/2390384.2390404> [Accessed 13 December 2021].




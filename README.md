# Compare Similarity for 14 translater in Surah (Al-Fatihah)
 
## Overview
This is a text mining project to determine that Surah(Al-Fatihah) is also be Al-Fatihah even translate different 14 translater.But as a computer,it does not know what is Surah(Al-Fatihah). So, this project is about to teach computer to understand about Al-Fatihah with text mining with some mathematical metrix through codeless mining tool.

<p float="left">
    <img src="images/workflow.png" alt="data" width="100"/>
</p>

## Data (Alquran english translation)
- Dr. Mustafa Khattab, the Clear Quran
- Fadel Soliman, Bridges’ translation
- Maarif-ul-Quran
- Mufti Taqi Usmani
- Dr. Ghali
- Abdul Haleem
- Tafheem-ul-Quran - Abul Ala Maududi
- English Translation (Pickthall)
- English Translation (Yusuf Ali)
- Ruwwad Center
- Dr. T. B. Irving
- Muhammad Taqi-ud-Din al-Hilali &amp; Muhammad Muhsin Khan
- Maulana Wahiduddin Khan
- Ibn_Kathir 

## Methodology

### Model
#### 1.[Term Frequency-Inverse Document Frequency (tf*idf)](https://en.wikipedia.org/wiki/Tf–idf)
#### 2.[Cosine Similarity](https://www.geeksforgeeks.org/cosine-similarity/)
#### 3.[Word2Vec](https://towardsdatascience.com/word2vec-explained-49c52b4ccb71)
#### 4.Text Preprocessing
 - Tokenized(tokenize all words)
 - Stopwords(clean all stopwords)
 - Tagger(tag the words according to dictionary)
 - lemmatization(change the words to their root words)

### Tools of use
- Knime
![](https://www.knime.com/themes/custom/bootstrap_knime/logo_black.svg)

### package in need
- Textproccessing (in knime)
 
### Steps
- Access Data
- Tranform Data
- Text preprocessing
- Model
- Measure similarity

#### Access Data
use the excel file in the datasets folder of this repository

#### Tranform Data

<p float="left">
    <img src="images/tranformworkflow.png" alt="data" width="100"/>
</p>

### Text preprocessing

#### For TF-IDF
<p float="left">
    <img src="images/textpre(tf-idf).png" alt="data" width="100"/>
</p>

#### For Word2Vec
<p float="left">
    <img src="images/Textpre(word2vec).png" alt="data" width="100"/>
</p>

### Model 

#### TF-IDF
<p float="left">
    <img src="images/Tfidf.png" alt="data" width="100"/>
</p>

#### Word2Vec
<p float="left">
    <img src="images/word2vecs.png" alt="data" width="100"/>
</p>

### Measure similarity

<p float="left">
    <img src="images/similarity.png" alt="data" width="100"/>
</p>

## Results
### Access data
<p float="left">
    <img src="images/data.png" alt="data" width="100"/>
</p>

### Tranform data
<p float="left">
    <img src="images/tranform.png" alt="data" width="100"/>
</p>

### Text Preprocessing
#### In TF-IDF

##### after preprocessing
<p float="left">
    <img src="images/tag.png" alt="data" width="100"/>
</p>

##### Bag of Word
<p float="left">
    <img src="images/Bagofword.png" alt="data" width="100"/>
</p>

#### In Word2Vec
##### after preprocessing
<p float="left">
    <img src="images/example.png" alt="data" width="100"/>
</p>

### Model
#### TF-IDF
<p float="left">
    <img src="images/tfidtmodel.png" alt="data" width="100"/>
</p>

##### Document vector
<p float="left">
    <img src="images/docvec.png" alt="data" width="100"/>
</p>

#### Word2Vec
##### Vocabulary
<p float="left">
    <img src="images/word2vecmodel.png" alt="data" width="100"/>
</p>

#### Document vector
<p float="left">
    <img src="images/docvector.png" alt="data" width="100"/>
</p>


### Mesure Similarity
#### Mesure TF-IDF model
<p float="left">
    <img src="images/table.png" alt="data" width="100"/>
</p>

##### Heatmap(TF-IDF)
<p float="left">
    <img src="images/heatmap.png" alt="data" width="100"/>
</p>

####  Mesure Word2Vec model
<p float="left">
    <img src="images/similartable.png" alt="data" width="100"/>
</p>

##### Heatmap(word2vec)
<p float="left">
    <img src="images/heatmap(word2vec).png" alt="data" width="100"/>
</p>

## Conclusion
   In this project, i use  TF-IDF and Word2Vec to create weight frequecy of words to measure
   the distance between 14 documents of surah Al-fatihah with cosine similarity. For conclusion, 
   we can see Word2Vec model give better result than TF-IDF model. TF-IDF model is only calculate
   weight of words depend on its appearance but Word2Vec model train the words to find relation
   with word vector.

## Suggestion
    TF-IDF model is suit for detect the documents(copy). And must use with other semantic model 
    and some dictionary such wordnet, glove to get better result.
    Word2Vec model is neutual network model so we must use large amount of dataset.

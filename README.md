# Compare Similarity for 14 translater in Surah (Al-Fatihah)
 
## Overview
This is a text mining project to determine that Surah(Al-Fatihah) is also be Al-Fatihah even translate different 14 translater.But as a computer,it does not know what is Surah(Al-Fatihah). So, this project is about to teach computer to understand about Al-Fatihah with text mining with some mathematical metrix through codeless mining tool.

![Imgur](https://i.imgur.com/NfvT4IG.png)

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
- TF-IDF
  ![Imgur](https://i.imgur.com/wjwSU2Q.png)
- Word2Vec
  
### Tools of use
- Knime
![](https://www.knime.com/themes/custom/bootstrap_knime/logo_black.svg)

### package in need
- Textproccessing (in knime)
 
### Steps
- Access Data
- Tranform Data
- Text preprocessing
- create model
- View the result

### Access Data
    use the excel file in the datasets folder of this repository

#### Tranform Data
    tranpose data 

    <p float="left">
       <img src="images/tranformworkflow.png" alt="data" width="500"/>
    </p>

### Text preprocessing

![Imgur](https://i.imgur.com/ZB4hCq4.png)

### Model 

![Imgur](https://i.imgur.com/wjwSU2Q.png)

## Use tf-idf model to calculate weight of words

![Imgur](https://i.imgur.com/E1nmjqa.png)

  
## Cosine similarity
 ### Example of cosine method usecase
![Imgur](https://i.imgur.com/i96p4GG.png)

## Use cosine similarity to see similarity or distance between documents

![Imgur](https://i.imgur.com/bAJSSM3.png)

# Conclusion
   In this project, i use tfi-df to create weight frequecy of words and use cosine method to measure
   the distance between 14 documents of surah Al-fatihah.And i got the highest similarity score- 0.85
   and the lowest one is - 0.14

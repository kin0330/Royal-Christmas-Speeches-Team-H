# Royal Christmas Speeches <br>

**1. About the repository**<br>
This repository contains materials of Group H’s group projects for the subjects Collecting Data and Tools and Methods.

**2. Introduction and background**<br>

***Historical background*** <br>
The Royal Christmas Messages have become a cherished tradition that dates back to 1932 when King George V delivered the very first Christmas message on the radio. Interestingly, it was Rudyard Kipling, the esteemed author of "The Jungle Book," who penned this inaugural Christmas speech. The King himself was not the originator of the idea; credit goes to Sir John Reith, a prominent figure at the British Broadcasting Company.<br>
The annual Christmas speech carries a highly personal touch. It is crafted by the monarchs themselves, sometimes with assistance from their cabinet, and serves as a heartfelt message addressed directly to the people. This annual tradition allows the monarch to connect with the public in a more intimate and personal manner.<br> 
In 1957, the Royal Christmas Message took another significant leap forward with the first-ever televised broadcast. From then until 1960, these Christmas speeches were broadcast live on television. However, starting in 1960, the messages were pre-recorded to allow for wider distribution across the Commonwealth. <br> 
The setting of these broadcasts played a crucial role in their impact. Not only could people see the Queen delivering her message, but they were also treated to a warm and inviting "homely" setting adorned with Christmas decorations. This deliberate choice of setting was part of the communication strategy, as it aimed to create a sense of relatability and connection with people throughout the country. By presenting herself in a familiar and festive environment, the Queen fostered a sense of intimacy and closeness with the viewers. <br>
The Corpus of Royal Christmas Speeches consists of a total of 70 speeches, encompassing the entirety of Queen Elizabeth II's reign up until her last Christmas speech in 2021. This extensive collection provides a valuable resource for studying the evolution of the monarchy's communication practices during the festive season. Additionally, the inclusion of the two speeches by King Charles III marks a significant transition within the monarchy, offering insights into the shifting dynamics of royal addresses. <br>

**3. Corpus**<br>
Our corpus includes the transcripts of Christmas speeches given by the British Queen Elizabeth II from 1952 to 2021 and her successor King Charles III in 2022 and 2023. The corpus consists of 72 speeches altogether.

**4. Target audience**<br>
The corpus is suitable for researchers who are interested in the Christmas messages given by the British royal family, especially in their analysis from a text-based perspective.

**5. Text selection criteria**<br>
We intended to gather the entirety of the Christmas speeches given by the late Queen Elizabeth II and her son’s, King Charles III’s, Christmas speeches that he has delivered up until now. We aimed to compare the current King’s speeches with those of the late Queen’s. The speeches comprise a homogeneous corpus.

**. Data collection process**<br>
The transcripts of the speeches were collected through web scraping from the [official website of the British Royal family](https://www.royal.uk/the-christmas-broadcast). We created a web crawler that goes through the links by formatting the string and saves the HTML files. After this the text is extracted using the Beautiful Soup library and saved in text files.

**8. Cleaning and pre-processing**<br>
The saved text files needed to be cleaned because they contained parts that we did not mean to analyze (abstract, introduction). Therefore, we manually annotated different sections of the transcripts (abstract, introduction, main part) to be able to carry out analyses on the main part. We saved the cleaned text in a CSV file, and the main text in txt files.<br>
We added further metadata to the csv file, such as where the speeches were given, when they were first broadcast on TV, etc.<br>
Finally, we saved the clean corpus and the metadata in the same CSV file.

**9. Dataset**<br>
We gathered data and created three datasets in the form of 2 csv files: data.csv, metadata.csv and enriched-corpus.csv.<br>

The ***metadata.csv*** file contains further information on the speeches, such as in which year they appeared, which monarch delivered the speech, the type of media that broadcast the speech, etc.<br>
| Columns | Descriptions |
| ------------- | ------------- |
| year | the year in which the speech was given |
| monarch | the name of the monarch by whom the speech was delivered |
| media | the type of media that broadcast the speech |
| channel | the name of the radio or TV channel that broadcast the speech |
| place | the location at which the speech was given |
| context | additional contextual information about the speech |

The ***enriched_corpus.csv*** incorporates all the information provided in the data.csv and metadata.csv and is further supplemented with lists of word tokens, sentence tokens and lemmas of the main text of each speech.
| Columns | Descriptions |
| ------------- | ------------- |
| year | the year in which the speech was given |
| monarch | the name of the monarch by whom the speech was delivered |
| media | the type of media that broadcast the speech |
| channel | the name of the radio or TV channel that broadcast the speech |
| place | the location at which the speech was given |
| context | additional contextual information about the speech |
| Title | the title of the speech |
| CleanedAbstract | the cleaned abstract section of the speech |
| AbstractWordCount | the number of words appearing in the abstract |
| CleanedIntro | the cleaned introduction section of the speech |
| IntroWordCount | the number of words appearing in the introduction |
| CleanedMainText | the cleaned main text section of the speech |
| MainTextWordCount | the number of words appearing in the main text |
| WordTokensMain | the word tokens of the main text section of the speech |
| SentenceTokensMain | the sentence tokens of the main text section of the speech |
| LemmasMain | the lemmas of the main text section of the speech |

**10. Research questions**<br>

***Collecting Data:***<br>1. Catsiapis (2005) mentions ‘family’, ’Commonwealth’ and ’Christmas’ as overarching themes in her close reading of the Queen’s Christmas speeches.<br>Can we identify the same themes with computational methods?<br>
2. When did the term 'empire' change to 'commonwealth'? And what terms are the most associated with both?<br>
3. What does readability analysis tell us?<br>


**11. Text analysis - Collecting Data**<br>
To answer our research questions for Collecting Data, we conducted a text analysis and employed the libraries (nltk for natural language processing, pandas for data manipulation and analysis, DataFrame and Series) and visualizations (matplotlib.pyplot) available in python.<br>

**13. Tutorial**<br>
We provide tutorials on the use of the web crawler, on the cleaning and pre-processing, and on text analysis using Python in the form of Jupyter Notebooks.<br>

**14. Active Learning Exercise**<br>
We created an active learning exercise on carrying out a sentiment analysis of the corpus. In the active learning exercises we use the VADER sentiment analyzer from the NLTK library. The exercises focus on the dissection of the emotional tone in each speech and tracking how these tones evolve in the speeches of Queen's and King's.

**15. Research output**<br>
To publish our findings, we created the following website: https://royal-christmas-messages.my.canva.site/

**16. Files in this repository**<br>
- `README.md` description of the repositor
- `christmas_speeches_webcrawler.ipynb` web crawler for downloading the HTML and text files
- `theme_analysis.ipynb` thematic analysis of speeches using keywords
- `processing_ALE.ipynb` preprocessing and creation of corpus & 
- csv file containing metadata on the Queen’s speeches (metadata.csv)
- csv file containing the cleaned speeches enriched with metadata on the Queen's speeches and with tokenized and lemmatized version of the main text section of the speeches (enriched_corpus.csv)
- data management plan (dmp.pdf)

**Contributors**<br>
Bente :rose:  Mathilde :sunflower: Mengying :leaves: Miriam :maple_leaf: Reka :evergreen_tree: Shiyan :herb: Yunchi :volcano:

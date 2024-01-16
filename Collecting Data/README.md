# Royal Christmas Speeches <br>

**1. About the folder**<br>
This folder contains materials of Group H’s group project for the subject Collecting Data.

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

**6. Data collection process**<br>
The transcripts of the speeches were collected through web scraping from the [official website of the British Royal family](https://www.royal.uk/the-christmas-broadcast). We created a web crawler that went through the links by formatting the string and saved the HTML files. After this, the text was extracted using the Beautiful Soup library and was saved in text files.

**7. Cleaning and pre-processing**<br>
The saved text files contained sections that we did not intend to analyze. Therefore, we manually annotated different sections of the transcripts - abstract, introduction, main text - so that we could focus on the main text part. We extracted and cleaned the three different sections, performed word counting and saved the results as a csv file. Then, we gathered further contextual metadata on the speeches (metadata.csv). Finally, we combined the information on the cleaned sections and the metadata, and enriched that corpus with word tokens, sentence tokens and lemmas of the main text part (enriched_corpus.csv).<br>

**8. Dataset**<br>
We gathered data and created datasets in the form of 2 csv files: metadata.csv and enriched_corpus.csv.<br>

The ***metadata.csv*** file contains further contextual information on the speeches, such as in which year they appeared, which monarch delivered the speech, the type of media that broadcast the speech, etc.<br>
| Columns | Descriptions |
| ------------- | ------------- |
| year | the year in which the speech was given |
| monarch | the name of the monarch by whom the speech was delivered |
| media | the type of media that broadcast the speech |
| channel | the name of the radio or TV channel that broadcast the speech |
| place | the location at which the speech was given |
| context | additional contextual information about the speech |

The ***enriched_corpus.csv*** incorporates all the information on the cleaned sections and the metadata, and is further supplemented with lists of word tokens, sentence tokens and lemmas of the main text of each speech.
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

**9. Research questions - Collecting Data**<br>
1. Catsiapis (2005) mentions ‘family’, ‘Commonwealth’ and ‘Christmas’ as overarching themes in her close reading of the Queen’s Christmas speeches.<br>Can we identify the same themes with computational methods?<br>
2. When did the term 'empire' change to 'commonwealth'? And what terms are the most associated with both?<br>
3. What does readability analysis tell us?<br>

Source:<br>
Catsiapis, H. 2005. The Queen's Christmas Messages. In Vernon, P. (Ed.), Seeing Things: literature and the visual : Papers from the Fifth International British Council Symposium, September 2001. Presses universitaires François-Rabelais. doi :10.4000/books.pufr.4223<br>

**10. Theme analysis - Collecting Data**<br>
To answer our research questions for Collecting Data, we conducted a text analysis and employed the libraries (nltk for natural language processing, pandas for data manipulation and analysis, DataFrame and Series) and visualizations (matplotlib.pyplot) available in Python.<br>

**11. Tutorial**<br>
We provided tutorials on web scraping, on cleaning and pre-processing, and on text analysis using Python in the form of Jupyter Notebooks.<br>

**12. Active Learning Exercise**<br>
We created an active learning exercise on carrying out a sentiment analysis of the corpus. In the active learning exercise we use the VADER sentiment analyzer from the NLTK library. The exercise focuses on the dissection of the emotional tone in each speech and tracking how these tones evolve in the Queen's speeches. Further, we invite readers to reflect on the limitations and capabilities of distant reading through this learning exercise.

**13. Research output**<br>
To publish our findings, we created the following website: https://royal-christmas-messages.my.canva.site/

**14. Files in this folder**<br>
- `README.md` description of the folder
- `christmas_speeches_webcrawler.ipynb` web crawler for downloading the HTML and text files
- `theme_analysis.ipynb` thematic analysis of speeches using keywords
- `processing_ALE.ipynb` preprocessing and creation of corpus & 
- `metadata.csv` csv file containing metadata on the Queen’s speeches 
- `enriched_corpus.csv` csv file containing the cleaned speeches enriched with metadata on the Queen's speeches and with tokenized and lemmatized version of the main text section of the speeches 
- `dmp.pdf` data management plan

**Contributors**<br>
Bente :rose:  Mathilde :sunflower: Mengying :leaves: Miriam :maple_leaf: Reka :evergreen_tree: Shiyan :herb: Yunchi :volcano:

# Royal Christmas Speeches <br>

**1. About the repository**<br>
This repository contains materials of Group H’s group projects for the subjects Collecting Data and Tools and Methods.

**2. Corpus**<br>
Our corpus includes the transcripts of Christmas speeches given by the British Queen Elizabeth II from 1952 to 2021 and her successor King Charles III in 2022 and 2023. The corpus consists of 72 speeches altogether.

**3. Target audience**<br>
The corpus is suitable for researchers who are interested in the Christmas messages given by the British royal family, especially in their analysis from a text-based perspective.

**4. Text selection criteria**<br>
We intended to gather the entirety of the Christmas speeches given by the late Queen Elizabeth II and her son’s, King Charles III’s, Christmas speeches that he has delivered up until now. We aimed to compare the current King’s speeches with those of the late Queen’s. The speeches comprise a homogeneous corpus.

**5. Objectives**<br>
a) answer our research questions<br>
b) provide a tutorial<br>
c) create active learning exercises<br>

**6. Data collection process**<br>
The transcripts of the speeches were collected through web scraping from the official website of the British Royal family (https://www.royal.uk/the-christmas-broadcast). We created a web crawler that goes through the links by formatting the string and saves the HTML files. After this the text is extracted using the Beautiful Soup library and saved in text files.



**7. Cleaning and pre-processing**<br>
The saved text files needed to be cleaned because they contained parts that we did not mean to analyze (abstract, introduction). Therefore, we manually annotated different sections of the transcripts (abstract, introduction, main part) to be able to carry out analyses on the main part. We saved the cleaned text in a CSV file, and the main text in txt files.<br>
We added further metadata to the csv file, such as where the speeches were given, when they were first broadcast on TV, etc.<br>
Finally, we saved the clean corpus and the metadata in the same CSV file.

**8. Research questions**<br>

***Collecting Data:***<br>
Are there any other keywords / key themes in the Queen’s Christmas speeches other than family, the Commonwealth and Christmas? 

***Tools and Methods:***<br>1. Does the style of the Queen’s Christmas speeches evolve over time or does it stay the same? <br>
2. Are King Charles III's speeches stylistically similar or dissimilar to Queen Elizabeth's Christmas speeches? <br>
3. a) What are the most used words by the Queen in 1952, 1953 and by the King in 2022, 2023? (a comparison of the Queen’s and the King’s first two speeches) <br>
b) What are the most used words by the Queen in 2020, 2021 and by the King in 2022, 2023? (a comparison of the last two speeches of the Queen and the first two speeches of the King, from the perspective of continuity)

**9. Collecting Data analysis**<br>

**10. Stylometric analysis**<br>
In order to answer our research questions for Tools and Methods, we carried out a stylometric analysis and utilized the Stylo package of R.<br>
We used Cluster Analysis and Craig's Zeta score and visualized the results in the form of dendrograms and graphs.

**11. Tutorial**<br>
We provide a tutorial on the use of the web crawler and on the cleaning and pre-processing in the form of Jupyter Notebooks.<br>
We also created a tutorial for the exploration of themes using the tool Voyant.

**12. Active Learning Exercises**<br>
We created active learning exercises on carrying out a sentiment analysis of the corpus.

**13. Research output**<br>
To publish our findings, we created the following website: https://royal-christmas-messages.my.canva.site/

**14. Files in this repository**<br>
- description of the repository and the group projects (README.md )
- Jupyter Notebook: first upload for the web crawler (queen_crawler.ipynb)
- Jupyter Notebook: cleaning and pre-processing the corpus (corpus_processing.ipynb)
- cleaned data csv (data.csv)
- fully pre-processed and enriched with metadata (enriched_corpus.csv)
- metadata on the Queen’s speeches (metadata.csv)
- report on the stylometric analysis of the corpus (….pdf)
- data management plan (….pdf)
- …

**Contributors**<br>
Bente :rose:  Mathilde :sunflower: Mengying :leaves: Miriam :maple_leaf: Reka :evergreen_tree: Shiyan :herb: Yunchi :volcano:

# WeChat



Type  | Value
----------- | -------------
Source | [211.159.163.137 - City: Beijing  - Country: China  - Organization: Tencent cloud computing](https://twitter.com/0xDUDE/status/1111338523670601729)
Description | [1.081.231.257 captured WeChat dialogues containing 3.784.309.399 messages dated 18 March 2019 were automatically selected for review based on a keyword trigger.](https://twitter.com/0xDUDE/status/1107793510881742848) Not all the dialogues were in Chinese or only had GPS coordinates in China.

## Project files:
 * MongoDB db.stats() `db.tencent.stats()`
 * MongoDB db.collection.stats() `db.tencent.wxmsg_20190318.stats()` 
 * MongoDB export `mongoexport --db tencent --collection wxmsg_20190318 --out wxmsg_20190318.json`
 * ~~Grep [output](#)~~
 * ~~Recovered [Jupyter notebook files]()~~
 * [Keywords](https://github.com/GDI-foundation/WeChat/blob/master/keywords.txt) used and found in the [wxmsg_20190318.json]() export file. 
 * [Chinese Stop Word list](https://github.com/cookiemonster/WeChat/blob/master/Chinese.stop.words.txt)
 * [English Stop Word list](https://github.com/cookiemonster/WeChat/blob/master/English.stop.words.txt)

## Natural Language Processing tools
* [Scikit-learn](https://scikit-learn.org)
* [NLTK](https://www.nltk.org/)
* [spaCy](https://spacy.io)

## Research files
* [Jupyter Notebook](https://jupyter.org/)
 
## Update
* January 2020: The Google Translate Toolkit service is down. The translated data is still attainable via [Google Takeout](https://takeout.google.com/?pli=1). The process of refactoring all the salvaged components into a new research project has started. 

* December 2019: We gave up brute-forcing the VerCrypt container and moved on to the data which was saved in screenshots and the data which was uploaded to [Google Translate Toolkit](translate.google.com/toolkit)

* [June 2019](https://twitter.com/0xDUDE/status/1138027431258918918?s=20): We got a small disk image of Ubuntu 18.04.2 desktop image,  which was used to build the Jupyter Notebook files. After many attempts to find any evidence on the system image, it became clear nothing was stored here. We found symlink a Veracrypt container, but we did not find a password that would open a hidden container. A simple password 'password' did open an empty container.

* [May 2019](https://twitter.com/GDI_FDN/status/1130489101273243648?s=20): We have lost access to the original data source. Also, the server with research data is not accessible anymore. Even, the Chinese student who was helping in building the Jupyter Notebook files (creating stop word lists, tokenization, lemmatization, and phrase matching) based on the WeChat dialogues

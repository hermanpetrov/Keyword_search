# Estonian Keyword Search

This tool was developed as a part of a Bachelor's thesis.

KEYWORD SEARCH IN ESTONIAN TEXTS

Tallinn University 2022

Estonian Keywords Search is a python interpreter tool which allows users to find keywords from estonian texts. The tool has an included reference corpus [(Estonian National Corpus 2021)](https://doi.org/10.15155/3-00-0000-0000-0000-08D1FL) made by the Institute of the Estonian language and a lemmatizer  to lemmatize both user provided reference or focus corpa.

The tool has included two focus corpa which are for learning and tool testing purposes.

The tool utilizes four different statistical methods for keyword calculation:
Log-likelihood
Chi-square
Log-ratio
Simple maths


To use the tool it is necessary to  run the script in Python 3.8 and install the following libraries:
  * Pandas (https://pandas.pydata.org) for data structuring.
  * Scipy (https://scipy.org) for computation.
  * Stanza (https://stanfordnlp.github.io/stanza/) for lemmatization.

## Quick guide

The main navigation around the tool is done by inputting the row numbers.

![MENU](https://user-images.githubusercontent.com/55134673/166155542-7dea63a6-a73a-42fe-88ca-5400d86bfa64.jpg)

### Corpus settings

![MENU_b](https://user-images.githubusercontent.com/55134673/166156066-4e68b084-d008-4574-96aa-79a48fdd2abb.jpg)

In the corpus settings the user is provided with the opportunity to select a both focus and reference corpa. 
The corpus creation depends from the purpose of the corpus.

Example: if the user decides to add another focus corpus then  before the corpus creation process, the provided corpus should be added to the focusCorpus folder. During the corpus creation the processed corpus is lemmatized and the words are extracted to the focusCorpusWords folder. After the corpus creation is complete the user can select their preffered focus corpus that will be used in the keyword calculations.


### Keyword search settings

![MENU_g](https://user-images.githubusercontent.com/55134673/166156057-e9f11b3d-a218-406f-aa59-3f99d114c6f0.jpg)

In the keyword search settings the user can adjust the settings of the resulting data. If the user decideds to use a large focus corpus then it is recommended to increase the minimal focus corpus word frequency. 

### Keyword search

![MENU_x](https://user-images.githubusercontent.com/55134673/166156590-70061b7a-c97e-4544-aa6e-08da0e8736ed.jpg)

The keyword search is the main function of the Estonian Keyword Search tool. 

![MENU_Y](https://user-images.githubusercontent.com/55134673/166156605-bcb25ae7-a6c2-4719-8f75-a3066317056f.jpg)

Upon initation the tool will begin to calcualte the keyword scores both with lemmatized and non lemmatized words. After the calculation is complete the used focus corpus keyword folder is created in the keynessValue folder. The created folder will be named both after the compared focus and reference corpus. 

![Folder](https://user-images.githubusercontent.com/55134673/166156645-bf485d1f-ed7c-4869-83dc-c0a3f1625c8d.PNG)

Inside the resulted keyness folder the user will be provided with scores calculated from all 4 above mentioned statistical methods for both lemmatized and non lemmatized words. 

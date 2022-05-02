# Estonian Keyword Search

This tool was developed as a part of a Bachelor's thesis.

KEYWORD SEARCH IN ESTONIAN TEXTS

Tallinn University 2022

Estonian Keywords Search is a python interpreter tool which allows users to find keywords from estonian texts. The tool has an included reference corpus [(Estonian National Corpus 2021)](https://doi.org/10.15155/3-00-0000-0000-0000-08D1FL) made by the Institute of the Estonian Language and a lemmatizer  to lemmatize both user provided reference and focus corpa.

The tool has included two focus corpa which are meant for the tool learning and testing purposes.

The tool utilizes four different statistical methods for keyword calculation:
* Log-likelihood
* Chi-square
* Log-ratio
* Simple maths


To use the tool it is necessary to  run the script in Python 3.8 and install the following libraries:
  * Pandas (https://pandas.pydata.org) for data structuring.
  * Scipy (https://scipy.org) for computation.
  * Stanza (https://stanfordnlp.github.io/stanza/) for lemmatization.

The tool is meant to be used only with estonian texts, any other language will be presented with inaccurate data.

## Quick guide

The main navigation around the tool is done by inputting the row numbers. 
Example: if the user would like to select the first option on the menu, the user should type in 1 and press enter.

![MENU](https://user-images.githubusercontent.com/55134673/166234891-9e23972f-cb47-4026-8c83-660ccb7b64f6.jpg)

### Corpus settings

![Menu_b (2)](https://user-images.githubusercontent.com/55134673/166234912-a418b93e-cec6-4af0-939d-c8f41b6da3b6.jpg)

In the corpus settings the user is provided with the opportunity to manage used focus and reference corpa. 

The corpus creation options allows for the user to create a new corpus wordlist. The creation of the wordlist depends from the purpose of the corpus.

Example: if the user decides to add another focus corpus then  before the corpus creation process, the provided corpus should be added to the focusCorpus folder. During the corpus creation the processed corpus is lemmatized and the resulted focus corpus wordlist folder will be returned in the focusCorpusWords. After the corpus creation is complete the user can select their preffered focus corpus that will be used in the keyword calculations.


### Keyword search settings

![MENU_g](https://user-images.githubusercontent.com/55134673/166156057-e9f11b3d-a218-406f-aa59-3f99d114c6f0.jpg)

In the keyword search settings the user can adjust the filters of the resulting data.

### Keyword search

![Menu_f (2)](https://user-images.githubusercontent.com/55134673/166234933-b7e47a8e-928e-41eb-99e8-f9bf6447a083.jpg)

The keyword search is the main function of the Estonian Keyword Search tool. 

![MENU_Y](https://user-images.githubusercontent.com/55134673/166156605-bcb25ae7-a6c2-4719-8f75-a3066317056f.jpg)

Upon initation the tool will begin to calcualte the keyword scores both with lemmatized and non lemmatized words. After the calculation is complete the used focus corpus keyword folder is created in the keynessValue folder. The created folder will be named both after the compared focus and reference corpus. 

![Folder](https://user-images.githubusercontent.com/55134673/166235904-86ffa26e-41a5-4568-8fa1-e3fbbe37ee27.PNG)

Inside the resulted keyness folder the user will be provided with scores calculated from all 4 above mentioned statistical methods for both lemmatized and non lemmatized words. 

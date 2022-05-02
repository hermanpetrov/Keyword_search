### Analysis of keyword methods

In the analysis folder I showcase the results of the used methods (Chi-square, Log-likelihood, Log-ratio, Simple maths). 
The focus point of the analysis was to establish which of the four methods:

* provide the most original keywords
* practical in keyword search

## Analysis based on score

From all four methods it is determined that there are problems with zero frequency words in keyword calculation.
Methods like Chi-square and Log-ratio suffer heavily from zero frequencies. The issue arises mostly from noise caused
by words with grammatical errors. Because words with grammatical errors can not be found in the reference corpus they are
determined to be uniqued for some methods even if they are not of any use.

Chi-square main problem is that zero frequency values are ranked with a high score above all other values. 
Log-ratio main problem is that zero frequency words get a score of infinity which causes a confusion around the scoreboard. Compared to chi-square the zero
frequency words are not ranked by any score. Meaning if there are actually unique words then user should manually analyze the scoreboard to understand whether
or not the provided infinity value words are keywords. 

Simple maths and log-likelihood suffer less from such problems yet still like in "Riigieksami_tulemused_MIN_1_sagedus" they are present in the first top 20 
lemmatized keywords.

The problem is even greater when it comes to comparison of even bigger corpa. In corpus K1 it is not possible to make a clear comparison of all four methods due to 
the big amount of noise.

### Frequency adjustment

Because of the great amount of noise the appropriate solution was to increase the minimum frequency of words in the focus corpa. In the analysis phase I tested
with increased minimal frequencies starting from 2 until 5. The higher the limit the less words were shown on the scoreboard. Because the aim was to minimize the amount
of noise the so called sweet spot depends from the corpus size. In this analysis it was found that minimum frequency of 2 was appropriate for Riigieksam material and 
minimum frequency of 5 for the K1 corpus. 

The adjusted minimum frequency brought out more similiarities between resulted choice of keywords therefore it was more appropriate to check the originiality of the provided
words.

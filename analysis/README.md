### Analysis of keyword methods

In the analysis folder, I showcase the results of the used methods (Chi-square, Log-likelihood, Log-ratio, Simple maths). 
The focus point of the analysis was to establish which of the four methods:

*are practical in a keyword search
*are providing the most original keywords


## Analysis based on the score

All four methods determined that there are problems with zero frequency words in keyword calculation. Methods like Chi-square and Log-ratio suffer heavily from zero frequencies. The issue arises primarily from noise caused by terms with grammatical errors. Because words with grammatical errors can not be found in the reference corpus, they are
determined to be unique for some methods, even if they are not significant.


Chi-square's main problem is that zero frequency values are ranked with a high score above all other values. 
Log-ratio's main problem is that zero frequency words get an infinity score. Compared to chi-square, the zero
frequency words are not ranked by any score. Meaning if there are actually unique words, then the user should manually analyze the scoreboard to understand whether or not the provided infinity value words are keywords. 

Simple maths and log-likelihood suffer less from such problems, yet still, like in "Riigieksami_tulemused_MIN_1_sagedus," they are present in the first top 20 lemmatized keywords.


The problem is even more significant when it comes to the comparison of even bigger corpora. In corpus K1, it is not possible to make a clear comparison of all four methods due to the significant amount of noise.

![Ma](https://user-images.githubusercontent.com/55134673/166296100-d3214fd6-99a2-466d-91ba-41ad2d036e72.PNG)

### Frequency adjustment

Because of the significant amount of noise, the appropriate solution was to increase the minimum frequency of words in the focus corpora. In the analysis phase, I tested with increased minimal frequencies starting from 2 until 5. The higher the limit, the fewer words were shown on the scoreboard. Because the aim was to minimize the amount of noise, the so-called sweet spot depends on the corpus size. In this analysis, it was found that a minimum frequency of 2 was appropriate for Riigieksam material and a minimum frequency of 5 for the K1 corpus. 

The adjusted minimum frequency brought out more similarities between the resulted choice of keywords; therefore, it was more appropriate to check the originality of the provided words.
words.

![ag](https://user-images.githubusercontent.com/55134673/166296120-65fc85a4-5e86-4c36-8683-ee0f4445481f.PNG)

##Analysis of top words

##Analysis of top words

After evaluating and solving the problem with keyword noise, the second objective was to find whether or not the top words were different or original between the four methods. Thanks to [Good Calculators](https://goodcalculators.com/venn-diagram-maker/), the comparison was made through a four circle Venn diagram.

The data was viewed with a minimum frequency of 1 for both focus corpora and then considered with the above-mentioned raised minimum frequencies.

The analysis of top words showed us that often the log-likelihood method had original keywords. The difference in words was compared, and it did not seem that log-likelihood had any false suggestions. The method which had zero original words throughout the viewed Venn diagrams was chi-square. The values for chi-square with the minimum frequency I did not account for as it was bad data for comparison. The noticeable factor about chi-square was that it often had common original words with log-likelihood.

Additionally, the analysis noted that significance and effect measure methods had their own unique words found as provided in the image below, which means that the top keywords can depend on the used measuring methods.

![Venn_chart (33)](https://user-images.githubusercontent.com/55134673/166298817-090b93fb-d715-410b-af24-a1eec49527a3.png)

## Conclusion

From the analyzed data and Venn diagrams, it was visible that log-likelihood and simple maths are more practical in calculating keywords. The opinion is based on situational practicality with zero frequency values and the ability to provide original words. 

In future development, it is most likely that chi-square and log-ratio will be dropped from the tool as it would only provide the user with duplicate values from other methods. 

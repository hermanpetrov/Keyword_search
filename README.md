# Keyword_search
The keyword search tool is a project which was made for my bachelor thesis. They main objective was to create keyword tool using the gathered infromation about corpus linguistics and popular statistical methods used in softwares like Antconc, Wordsmith and Lancsbox. Additionally I checked also Sketch Engine as it is one of the biggest online text analysis tools to this date (2022). 

Objective of this tool was to determine which of the 4 methods provides less duplicate keywords and which methods provide us with the most original ones.

Key statistical methods that were analyzed:

Log-likelihood
Chi-square
Log-ratio
Simple maths

### Installation

Copy the repository to your device.

The keyword tool runs on Python 3.8. 
The main script requires the following imports
1.pandas
2.scipy
3.stanza

Suggested installation would be using PyPI:

For pandas: 
```
pip install pandas
```
For scipy: 
```
pip install scipy
```
For scipy: 
```
pip install stanza
```

Alternatively you can use the script with [Anaconda](https://www.anaconda.com/download) prompt. 

You can copy the repository through anaconda to your device with git.
In case git is not installed run the command:
```
conda install git
```
Cloning command:
```
git clone "URL"
```
Since the keyword tool runs on python version 3.8 it is recommended to create a python 3.8 environment.
```
conda create -n py38 python=3.8
```
To activate the environment: 
```
conda activate py38
```
After activating the environment make sure to run the same pip commands for the imports. 

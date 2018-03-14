# BUPA: Liver Disorders Data Set Analysis
## Introduction
BUPA data set contains the data of patients having the liver disorders. The first 5 variables are all blood tests which are thought to be sensitive to liver disorders that might arise from excessive alcohol consumption. Each line in the bupa.data file constitutes the record of a single male individual.

<b>Dataset statistics</b>
<pre>
  Data Set Characteristics: Multivariate
  Number of Instances: 345
  Area: Life
  Attribute Characteristics: Categorical, Integer, Real
  Number of Attributes: 7
  Date Donated: 1990-05-15
  Associated Tasks: N/A
  Missing Values? No
</pre>

<b>Data Fields Explanation</b>
<pre>
  1. mcv  - mean corpuscular volume
  2. alkphos  -	alkaline phosphotase
  3. sgpt -	alamine aminotransferase
  4. sgot - 	aspartate aminotransferase
  5. gammagt  -	gamma-glutamyl transpeptidase
  6. drinks -	number of half-pint equivalents of alcoholic beverages drunk per day
  7. selector -	field used to split data into two sets
</pre>
<b>NOTE:</b><br />
The final variable in the dataset is a train/test indicator, not a classification label.<br /><br />
A large majority of surveyed papers misinterpret the final column, with meaningless results.

## Misinterpretation of BUPA Dataset
As stated, in the Liver data set, x6 is a dependent variable indicating number of drinks, while x7 is a selector, intended to split the data into train and test subsets for one particular experiment. However, many papers interpret x6 as an independent variable, and x7 as the target for classification. In some cases it is explicitly claimed that x7 represents the presence or absence of a liver disorder. This is incorrect. In fact, the information in this data set which pertains to diagnosis is in the first five variables x1 to x5, which are the results of blood tests a physician might use to inform diagnosis. There is no ground truth in the data set relating to presence or absence of a disorder. Papers which blindly use x7 as a binary target are not doing what the researchers intend.

REFERENCE: https://www.richardsandesforsyth.net/pubs/JMRF_DiagnosingDisorder_PRL2016.pdf

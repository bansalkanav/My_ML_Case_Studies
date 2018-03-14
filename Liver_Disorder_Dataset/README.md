# BUPA: Liver Disorders Data Set Analysis
## Introduction
BUPA data set contains the data of patients having the liver disorders

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

## Misinterpretation of BUPA Dataset
As stated, in the Liver data set, x6 is a dependent variable indicating number of drinks, while x7 is a selector, intended to split the data into train and test subsets for one particular experiment. However, many papers interpret x6 as an independent variable, and x7 as the target for classification. In some cases it is explicitly claimed that x7 represents the presence or absence of a liver disorder. This is incorrect. In fact, the information in this data set which pertains to diagnosis is in the first five variables x1 to x5, which are the results of blood tests a physician might use to inform diagnosis. There is no ground truth in the data set relating to presence or absence of a disorder. Papers which blindly use x7 as a binary target are not doing what the researchers intend.

REFERENCE: https://www.richardsandesforsyth.net/pubs/JMRF_DiagnosingDisorder_PRL2016.pdf

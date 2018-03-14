# StackOverflow_Tag_Prediction
#### (A Multi-Label Classification Problem)

## Introduction
Stack Overflow is the largest, most trusted online community for developers to learn, share their programming knowledge, and build their careers.<br /><br />
	
Stack Overflow is something which every programmer use one way or another. Each month, over 50 million developers come to Stack Overflow to learn, share their knowledge, and build their careers. It features questions and answers on a wide range of topics in computer programming. The website serves as a platform for users to ask and answer questions, and, through membership and active participation, to vote questions and answers up or down and edit questions and answers in a fashion similar to a wiki or Digg. As of April 2014 Stack Overflow has over 4,000,000 registered users, and it exceeded 10,000,000 questions in late August 2015. Based on the type of tags assigned to questions, the top eight most discussed topics on the site are: Java, JavaScript, C#, PHP, Android, jQuery, Python and HTML.<br /><br />

<b>Data Set</b><br />
<a href="https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data">Click here</a> to get the dataset.<br />
The dataset of questions is obtained from a Kaggle competition [FB-Kaggle 2013]. The training set is 7 GB in size(after unzipping). The dataset contains over 6,034,195 questions and 42,049 unique tags.
The test set is 2GB in size and contains over 2 million questions. Each question in the training set contains four features - id, title, body and tags.<br /><br />

<b>Dataset statistics</b>
<pre>
    Data Type: CSV Files
    Data Size: Train – 7GB, Test – 2GB
    Train.csv features – id, title, body & tag
    Test.csv features – id, title & body
</pre>

<b>Data Fields Explanation</b>
Dataset contains 6034195 rows. The column in the table are:
<pre>
    Id - Unique identifier for each question
    Title - The question's title
    Body - The body of the question
    Tags - The tags associated with the question (all lowercase, should not contain tabs '\t' or ampersands '&')
</pre>

## EDA Objective
Analysing the data and plot the required graphs to show that these conclusions are True:
<pre>
    a. Presence of Redundant information.
    b. Questions Consists of text and code.
    c. More than 200 tags were used in at least 10,000 questions.
    d. Total of more than 33M unique words are present in the data.
    e. Majority of the most frequent tags were programming language.
    f. More than 50% of questions contain <code> tag.
</pre>
We are also interested to find:
<pre>
    a. Total number of questions?
    b. Average question size?
    c. Minimum and maximum number of tags per question?
    d. Average number of tags per question?
    e. Unique Tags
    f. Top 20 tags?
</pre>

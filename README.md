# Quora-Question-Pair-Similarity

![0_t8wHkI-8hKt1M-Sb](https://user-images.githubusercontent.com/115543070/205617646-c0357f53-ff8e-4569-a6a0-e9b368be9b18.png)

<h3> Description </h3>
Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. This empowers people to learn from each other and to better understand the world.

Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

<h3> Problem Statemen <\h3>

Identify which questions asked on Quora are duplicates of questions that have already been asked.

This could be useful to instantly provide answers to questions that have already been answered.

We are tasked with predicting whether a pair of questions are duplicates or not.

  <h3>Dataset Link<\h3>
Source : https://www.kaggle.com/c/quora-question-pairs

<h3> Objective and Constraints </h3>
It is a binary classification problem, for a given pair of questions we need to predict if they are duplicate or not.

The cost of a mis-classification can be very high.
    
You would want a probability of a pair of questions to be duplicates so that you can choose any threshold of choice.
    
No strict latency concerns.
    
Interpretability is partially important.
    
<h3> Data Overview </h3>
- Data will be in a file Train.csv

- Train.csv contains 5 columns : qid1, qid2, question1, question2, is_duplicate

- Size of Train.csv - 60MB

- Number of rows in Train.csv = 404,290

<h4> Example Data point </h4>
"id","qid1","qid2","question1","question2","is_duplicate"

"0","1","2","What is the step by step guide to invest in share market in india?","What is the step by step guide to invest in share market?","0"

"1","3","4","What is the story of Kohinoor (Koh-i-Noor) Diamond?","What would happen if the Indian government stole the Kohinoor (Koh-i-Noor) diamond back?","0"

"7","15","16","How can I be a good geologist?","What should I do to be a great geologist?","1"

"11","23","24","How do I read and find my YouTube comments?","How can I see all my Youtube comments?","1"


<h3>Performance Metric</h3>

Source: https://www.kaggle.com/c/quora-question-pairs#evaluation

log-loss : https://www.kaggle.com/wiki/LogarithmicLoss


# datasets

This repository contains datasets for evaluation, training and research of AI and Islam. It currently contains the following datasets. 

## BATIK

BATIK (Broad Automated Test of Islamic Knowledge) is a set of 100 questions and answers. 
The questions are factual questions extracted from the set of the first 2500 questions 
people have asked Ansari. It is a multiple choice quiz with each question having between 2 and 5 choices.

It is a multilingual test, with the test available in English, Arabic and Turkish. There is also a notebook (score-batik.ipynb)
for evlauating the results of different LLMs that also prints the errors made by each model. 

A cut-down version of the BATIK questions for humans (with all the Qur'an search questions removed, e.g. 
"Which verse of the Qur'an tells us how many angels are guardians over hell?", since that would be difficult for a human to answer) 
can be found [here](https://quizizz.com/join?gc=83764841) if you would like to try it. 

### Results

- Language does not seem to make a difference of accuracy. On both gpt-4o and gpt-4o-mini, the results in English, Arabic and Turkish are almost identical. 
- Using Ansari or using OpenAI's gpt-4o doesn't materially change the accuracy in these types of factual questions.
- This does not mean Ansari has no value -- Ansari is considerably better when it comes to referencing; it is just that this 
- OpenAI's gpt-4o gets 99% or 100% accuracy (there is some non-determinism in the answers).
- OpenAI's gpt-4o-mini gets 89% or 90% (there is some non-determinism).
- Humans completing the simplified quiz get a mean of 81% (note: small sample size of 5). 



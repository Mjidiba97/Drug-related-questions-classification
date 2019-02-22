# Drug-related questions classification, a challenge by POSOS
### By Ahmed Amine MAJDOUBI
---
***Important note:*** This is a challenge made by the company POSOS in 2018. Here is the original ***[link](https://www.college-de-france.fr/site/stephane-mallat/Challenge-2017-2018-Reponses-a-des-questions-pharmaceutiques-par-Posos.htm)*** for the challenge. POSOS is an NLP start-up aiming at answering questions about medication from non-structured biomedical sources. The goal of Posos challenge is to predict for each question the associated intent.

## Challenge Context

More than 6,000 different drugs are commercialized in France. Not only patients but also healthcare professionals remain unable to use them correctly when they do not have immediate access to appropriate information they may seek. Medicines remain responsible for more than 144,000 hospitalizations every year in France while in the United States, 1.5 million people face drug misuse every year. Questions about drug prescription, dispensation or use should never remain unanswered. What is particularly interesting to understand about drug queries is what information people expect to get as an answer: for instance, associated side effects, ingredients or contra-indications. Millions of queries are asked every year about drugs. There is a limited number of query types but the same question could be asked in many ways. Therefore, understanding what information people expect to get when asking a question is a great challenge.


## Data description

  The input data ***input_train.csv*** is a list of questions written in French. Each line is constituted with a unique ID followed by one question. In the input file, the first line is the header. Columns are separated by , characters. They correspond to: ID: line number. It relates to the line number in the output file. question: the question whose intent has to be predicted. Here below is an example of the input file content:

  *   Est-ce qu'il existe une forme adaptée aux enfants de 5ans du Micropakine ?
  *   laroxyl à doses faibles pour le stress
  *   mon psy me dit de prendre 50mg de sertraline le matin et 50 mg de sertraline le soir. Peut-on prendre 100mg soit le matin ou à midi

The output file ***output_train.csv*** contains the intent associated to each ID. The first line is the header; columns are always separated by , characters. They correspond to the line number and the intent identification number:

A list of 50 different intents has been predefined. We anonymized them for this challenge converting intents to identification numbers.Intents are homogeneously distributed between training and test files.
From the input_test.csv file, competitors will provide an ***output_test.csv*** file with the same format as the ***output_train.csv*** file. They will predict for each line number, the associated intent number.

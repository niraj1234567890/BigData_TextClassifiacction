# BigData_TextClassifiacction
Text classifaiction in a very large dataset is overwhelming,we have to extract some limited text data from this large dataset and then use it properly to classify the text.

## Context of the Dataset
Posts extracted from a Gitter's public chatroom used for an online course to learn to program.

The files contains the posts from students, bots, moderators and contributors in the main ("/freeCodeCamp") Gitter chatroom between 31-Dec-2014 until the first days of Dec-2017. There are around 5 million posts from near 400,000 users (all estimates). Data was extracted using Python code over the Gitter API. Records are not anonymised or modified and are presented "as they are".

The datasets are a contribution from freeCodeCamp as part of the freeCodeCamp's Open Data Initiative. More information about the rationale of this initiative can be found in this announcement of us releasing the chat history dataset.

Details about the structure of each post can be found at Gitter Rest-API documentation

Dataset for this problem can be found on Kaggle.

## Problem_Statment:
There are two categories of computer language.one is Python and another one is Java.We have to clasify user's message into these two categories.

## Approch to this text classfication problem
1. We are not going to use all of the messages from all the users instead we use most active user's messages.Now we have less text data so that we don't have to worry about the memory of a computer.
2. Make two dictionaries using Java's commen keywords(exp-css,html,js) and Python's commen keywords(exp-python,py,sklearn) respectively.
3. Extract only those messages from the above text data which are containing these java's and python's keywords and create a new dataset using only these messages.
4. Use CountVectorizer and TfidfVectorizer models to convert words into their vector forms and then train them with RandomForest Classifier and XGBoost Classifier respectively.

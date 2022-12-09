# Parsing-Analysis

# Overview

This parsing analysis is a quick exercising in finding the most popular Subject Verb Object combinations in a sample of Convention Speech text. To aid this analysis I will be using SpaCy as well as a Subject Object extraction py file that I did not write.

# Process

We'll begin with the Democratic text, querying a sample of speeches from our SQL database. From here we will append the query results to our convention data list within a for loop. For SpaCy SVO compatibility we will turn our list into one long string, remove punctuation, tokenize, and case fold / clean the text.

Next we'll load our parser into our file and call it on our long democratic string. We'll then use the find SVO's feature to find all the Subject Verb Object combinations in our democratic string. Finally, we'll use a counter to find the most common SVO's and print the top 25 to the screen.

Repeat the above steps for the Republican Party and compare.

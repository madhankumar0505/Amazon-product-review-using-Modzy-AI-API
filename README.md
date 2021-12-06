# Amazon-product-review-using-Modzy-AI-API

Link for demo: https://youtu.be/bhIBwuEyWEg
## Inspiration
I have seen _Amazon product reviews_ where customers' star rating doesn't seem to match with their text reviews. Hence I felt it is also important to convert text reviews into numeric data and provide a score that is a combination of star rating and text reviews.

## What it does
The link of the product review is fed as input to the model and output is **sentiScore** of the product. It uses web-scraping and **Modzy AI text summarization** and **Modzy AI sentiment analysis** to produce the output.

**what is sentiScore?**:
           sentiScore is calculated by combining 75% of the average star rating and 25% of the average of the product review's sentiment.

## How I built it
**1**.The first thing I had to do was web scraping Amazon product reviews. For this I used beautifulSoup python package.
**2**.The second step was to pre-prcoess the data scraped from reviews. For this I used regex to remove numericals from the reviews and nltk's stop words to remove unwanted words from reviews. Then I stored the data into a dataframe using pandas.
**3**.Next I created two functions . One for **Modzy AI text summarization API** and the other for **Modzy AI sentiment analysis**. Then stored the positive, negative and neutral scores in individual lists.
**4**. As the final step, I combined 75% of average of star rating and 25% average of sentiment score to get the final sentiScore.

## Challenges I ran into
**1**.Without using Modzy AI text summarization I couldn't achieve the desired results.
**2**.Numericals were a problem until I used regex
**3**.I was new to web scraping. Hence had to face issues while scraping data and preprocessing them.

## Accomplishments that I am proud of
I am proud of every small accomplishment I made in this project. Web scraping , integrating Modzy AI API 's and generating the sentiScore. were all part of my accomplishment.

## What I learned
I learned a new skill: web scraping. 
I improved my coding knowledge. 
I learned to use API's.
I explored different use cases of Modzy AI's API service.

## What's next for Amazon product reviews - sentiment analysis
**1**.I am going to improve the model's accuracy by using NLP BERT. 

**2**.I wanted to create a web application for this project. Since I am not good at web development I have included this for future development. 

**3**.In this user friendly web  application people can enter the product name to view it's sentiScore. This will also include features like comparing sentiScore of different brands of same product so that people can choose the best brand for the product they wish to purchase.

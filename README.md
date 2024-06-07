#  Сlustering of jokes by topic
HSE SPb machine learning basics project (Spring 2024)

### Team:
- Emelyanova Anastasia
- Saifutdinov Timur

## [Presentation](https://docs.google.com/presentation/d/1hta789Ms5h0oLUqHwKFAq8_q5rm1EVKiYzeo4hbNsDo)

##  Data description
Source dataset was found via random walk around Telegram. It is a csv file containing one column -- joke and 122081 rows.

## Our purposes
Train a model to cluster jokes by topics.

## Used algorithms

- For preprocessing, we've removed special characters, numbers, stop words, punctuation marks and converted to lower case
Lemmatized using pymorphy2 (analog - natasha, it was slower, same quality)
We removed top 10 frequent neutral words and words that occur in less than 3 anecdotes.
- BOW was chosen because the average anecdote contains 60 characters, which is generally not much, so the simplicity and speed of BOW is more important than the inconsequential advantage of TF-IDF.
- For clustering we chose LDA.

## Results
There is a google disc with results of our work:
- [disc](https://drive.google.com/drive/u/0/folders/1rmSZtXQ64Cp6pvJSBm5eSweOQ3toC5I5)

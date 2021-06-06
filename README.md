# Basic-NN-for-NLP
First time creating a neural network to do NLP. The process is basic, I download a database of tweets tagged in four categories: 'sports', 'politics', 'medical', 'entertainment'.   

First I process the text of the tweets using regular expressions to remove as much noise as possible from each tweet. In between, I remove mentions to other users, links, retweets and other objects. A good practice to visualize if you are cleaning things right is to plot the count of words for each target and see if they differ.I also rely on the stopwords of the nltk library.  

After cleaning the texts I proceed to form a bag of words (BOW) where I make a counter for each occurrence of that word in the user's text, changing the dimension of the array to nxk, where n is the number of users and k the number of words that exist in the entire sample after cleaning.  Finally I make a neural network that tries to classify each text into one of the 4 categories above. This does not have a bad performance (79% accuracy in the test sample), but tuning the hyperparameters of the neural network is something I am still learning.

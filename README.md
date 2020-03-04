<h2>Abstract</h2>
<p>
  Discussing things you care about can be difficult. The threat of abuse and harassment online means that many people stop expressing themselves and give up on seeking different opinions. Platforms struggle to effectively facilitate conversations, leading many communities to limit or completely shut down user comments.

The Conversation AI team, a research initiative founded by Jigsaw and Google (both a part of Alphabet) are working on tools to help improve online conversation. One area of focus is the study of negative online behaviors, like toxic comments (i.e. comments that are rude, disrespectful or otherwise likely to make someone leave a discussion). So far they’ve built a range of publicly available models served through the Perspective API, including toxicity. But the current models still make errors, and they don’t allow users to select which types of toxicity they’re interested in finding (e.g. some platforms may be fine with profanity, but not with other types of toxic content).

In this competition, you’re challenged to build a multi-headed model that’s capable of detecting different types of of toxicity like threats, obscenity, insults, and identity-based hate better than Perspective’s current models. You’ll be using a dataset of comments from Wikipedia’s talk page edits. Improvements to the current model will hopefully help online discussion become more productive and respectful.
</p>
<br>
<h2>Dataset</h2>
<p>You are provided with a large number of Wikipedia comments which have been labeled by human raters for toxic behavior. The types of toxicity are:

toxic<br>
severe_toxic<br>
obscene<br>
threat<br>
insult<br>
identity_hate<br>
You must create a model which predicts a probability of each type of toxicity for each comment.

File descriptions<br>
train.csv - the training set, contains comments with their binary labels<br>
test.csv - the test set, you must predict the toxicity probabilities for these comments. To deter hand labeling, the test set contains some comments which are not included in scoring.
sample_submission.csv - a sample submission file in the correct format<br>
test_labels.csv - labels for the test data; value of -1 indicates it was not used for scoring; (Note: file added after competition close!)</p>
<br>

<h2>Installation</h2>
<p>
  pip install cv2<br>
  pip install keras<br>
  pip install matplotlib<br>
  pip install numpy <br>
  pip install pandas<br>
  pip install seaborn<br>
  
</p>
<h2>Model: LSTM with pretrained Glove Embeddings</h2>
<h2>Accuracy: 98%</h2>

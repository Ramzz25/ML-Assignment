# ML-Assignment

## Problem Statement (option 1) :  
Crawl news & information websites & anticipate the likelihood of its virality. <br>

## My Approach : <br>
For this PS, I have scrapped the news headlines from the India Today website. I chose this website, because it shows trending news from the past week and one can also see the current news. Also, scrapping was easier to do in this website. <br>
After scrapping, I got 360 datapoints in total for training & validation -> 180 trending news + 180 general news (this was the maximum cap of news shown in the website). Also, got 120 current news headlines to make predictions. <br>
Then, after pre-processing the news headlines (methods of pre-processing are mentioned in the notebook), trained a *Logisic Regression* model on ~70% of the data. Achieved a validation f1-score and accuracy of 0.971 and 0.972 respectively. <br>
Finally, using the trained model predicted the probability of a news (current news) becoming viral.

## Methods to improve the model : <br>
This model is built only using 360 datapoints which is awfully less, which in turn is responsible for the higher accuracy. For a more generalized model, number of datapoints should be increased. This can be done by scrapping news from various popular websites like NDTV, The Hindu, LiveMint, TOI, etc.<br>
And better results can be achieved by using State-of-the-Art Neural Networks like *Transformers* (Ex : Google's BERT) rather than using classic ML algorithms.<br>
Also, isntead of quantifying the virality as a probability, we can predict how many views/shares a article would get given a certain period of time, as this would make both our model and result more interpretable.

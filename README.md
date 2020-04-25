# ML-Assignment

## Problem Statement (option 1) :  
Crawl news & information websites & anticipate the likelihood of its virality. <br>

## Approach : <br>
I have scrapped the news headlines from the India Today website. I chose this website, because it shows trending news from the past week and one can also see the current news. Also, scrapping was easier to do in this website. <br>
After scrapping, I got 360 datapoints in total for training & validation - 180 trending news + 180 general news. Also, got 120 current news headlines to make predictions. <br>
Then, after pre-processing the news headlines (methods of pre-processing are mentioned in the notebook), trained a 'Logisic Regression' model on ~70% of the data. Achieved a validation f1-score and accuracy of 0.971 and 0.972 respectively. <br>
Finally, using the trained model predicted the probability of a news (current news) becoming viral.

# RNN_Sentiment_Analysis
Sentiment Analysis/Opinion Mining using LSTM

Movie reviews from IMDb Dataset from "Learning Word Vectors for Sentiment Analysis", Maas et al, Proceedings of the 49th Annual Meeting of the Association for Computational Linguistics: Human Language Technologies, pages 142-150, Portland, Oregon, USA, Association for Computational Linguistics, June 2011


* 50000 reviews
* 1 and 0 labels (sentiment for positive and negative respectively)
* Train-Test split: 4 to 1
* 1 LSTM layer, 1 Dense Layer
* Dropout: 0.5 at the output     
* Binary Cross Entropy Loss function    
* Adam Optimizer(learning rate: .001)
* Batch size: 100
* Epochs: 10
* Embed size = 200, LSTM size = 256, Stateful = True - Train data accuracy: 99%; Test data accuracy: 87% => Overfitting
* Embed size = 200, LSTM size = 256, Stateful = False - Train data accuracy: 99%; Test data accuracy: 87% => Overfitting
* Embed size = 200, LSTM size = 64, Stateful = False - Train data accuracy: 99%; Test data accuracy: 88% => Still overfitting
* Requires regularization to reduce overfitting
* Embed size = 50, LSTM size = 64; L2 Regularization: 0.01, Stateful = False - Train data accuracy: 98%; Test data accuracy: 86% => Still overfitting

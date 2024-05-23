# NLP-ABSA

Aspect Based Sentiment Analysis

Aspect Based Sentiment Analysis (ABSA), is an advanced NLP task that aim to identify aspect terms (entities that expressed in text) present in 
the given review sentence, and predict the sentiment (e.g. positive, negative, neutral) associated with those aspects (Punitha, et al. 2023). 

This is more challenging comparing with the traditional sentences / article-based sentiment detection, where the task aims to predict an overall 
global sentiment only. While the overall sentiment is valuable, in many real practises, a single sentence (e.g. restaurant review) usually includes
different sentiments addressing different aspects. It would be significantly more beneficial, by gaining a deeper understanding of the sentiment
polarities, specifically to the aspect addressed (e.g. service, food, price etc).

This report has explored different recurrent neural network architectures with novel variants. The models were trained with MAMS 
(MultiAspect Multi-Sentiment) dataset (restaurant reviews), where each review sentence has at least two aspects mentioned with different sentiment 
polarities. 

The models aim to predict the sentiment polarities based on the corresponding review sentences, as well as the given aspects. 

The best performing model architect utilised the attention mechanism that figured out the relevant significant words, which helps to determine
sentiment polarities related to the aspect expressed. The quantitative and qualitative analysis have proved the attention mechanisms’
effectiveness, compared to the simple aspect embedding techniques. The best proposed model achieved 76.91% accuracy score in testing dataset, 
with respectively well performing F1-score in all three target sentiment classes: 76.75% (Negative), 80.71% (Neutral), and 70.83% (Positive).

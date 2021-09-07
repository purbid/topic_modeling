# topic_modeling
notebooks for topic modeling using BOW, TOP2VEC and BERTopic



These two noetbooks give various approaches to topic modeling. 
The topic_modeling_bow file shows topic modeling with BOW and LDA, followed by Top2Vec, a vector based model that uses Doc2Vec for Topic Modeling.
Results were much better with BOW LDA, with optimal number of topics 14. I took coherence scores to get to this number.
The viz looks as follows:
<img width="664" alt="bow_topic_model" src="https://user-images.githubusercontent.com/33604354/132368569-d8c5fe0b-c7d4-4d11-9a36-66fdb9dafc28.PNG">



The next file uses a BERT based model BERTopic for topic modeling. On its own, model finds 600+ topics.
Most of them are overlapping, hence we do some reduction in number of topics by merging similar topics together, to bring down the number of topics to 20.
The quality of extraction is much better than BOW LDA model, with niche topics like international Brexit, Immigration, Olympics, etc being identified. 
We should be able to furthur generalise and reduce the number of topics, if we wish to do so.
The viz looks as follows:
<img width="392" alt="bert_topic_model" src="https://user-images.githubusercontent.com/33604354/132369060-d4e6d2fd-a012-4497-9678-70315d4af542.PNG">
Even though it looks like there are a lot of overlapping topics, on zooming in we can see these are mutually exclusive topics and very niche topics.
As mentioned above, we can reduce the number of topics and increase the size of these topics/bubbles


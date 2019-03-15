# Datasets


### Criteo
[A Kaggle dataset for Criteo display advertising challenge](https://www.kaggle.com/c/criteo-display-ad-challenge/data) 

[Criteo](https://www.criteo.com/) is a personalized retargeting company that works with Internet retailers to serve personalized online display advertisements to consumers. The goal of this Kaggle challenge is to predict click-through rates on display ads. It offers a week’s worth of data from Criteo's traffic to develop and benchmark CTR prediction models. In the labeled training set over over a period of 7 days, each row corresponds to a display ad served by Criteo. Positive (clicked) and negatives (non-clicked) samples have both been subsampled at different rates in order to reduce the dataset size. The samples are chronologically ordered. The raw dataset is currently available for downloading at [here](https://s3-eu-west-1.amazonaws.com/kaggle-display-advertising-challenge-dataset/dac.tar.gz).

Note that we only use the labeled part of data as our benchmarking set. We split the data sequentially similar to the challenge. Since the timestamps are not shown, we use the same number of samples with the test set in the challenge. Therefore, we take the last 6,042,135 samples (w.r.t. the last day) for testing and the remaining samples for training and validation (w.r.t. the first 6 days).

Data fields:
+ Label - Target variable that indicates if an ad was clicked (1) or not (0).
+ I1-I13 - A total of 13 columns of integer features (mostly count features).
+ C1-C26 - A total of 26 columns of categorical features. The values of these features have been hashed onto 32 bits for anonymization purposes. 

### Avazu
[A Kaggle dataset for Avazu CTR prediction challenge](https://www.kaggle.com/c/avazu-ctr-prediction/data) 

[Avazu](http://avazuinc.com/home/) is one of the leading mobile advertising platforms globally. This Kaggle competition targets at predicting whether a mobile ad will be clicked and has provided 11 days worth of Avazu data to build and test prediction models. It consists of 10 days of labeled click-through data for training and 1 day of unlabeled ads data for testing.

Note that we only use the first 10 days of labeled data as our benchmarking set. We split the data sequentially similar to the challenge. That is, the first 9 days of data for training and validation (20141021~20141029), and the last day of data for testing (20141030).

Data fields:
+ id: ad identifier
+ click: 0/1 for non-click/click
+ hour: format is YYMMDDHH, so 14091123 means 23:00 on Sept. 11, 2014 UTC.
+ C1 -- anonymized categorical variable
+ banner_pos
+ site_id
+ site_domain
+ site_category
+ app_id
+ app_domain
+ app_category
+ device_id
+ device_ip
+ device_model
+ device_type
+ device_conn_type
+ C14-C21 -- anonymized categorical variables



### iPinyou
 [A real-time bidding algorithm competition dataset from iPinyou](http://contest.ipinyou.com/) 

### Taobao
[An ad display/click dataset from Taobao.com](https://tianchi.aliyun.com/datalab/dataSet.html?spm=5176.100073.0.0.14b66fc1ZofS5A&dataId=56)

### AliCCP

[A click dataset gathered from the recommender system in Taobao](https://tianchi.aliyun.com/datalab/dataSet.html?dataId=408) 

### Frappe
[A dataset for context-aware app recommendation in Frappe](https://arxiv.org/abs/1505.03014) 

### Other related datasets

+ Recommendation
    + [Amazon](http://jmcauley.ucsd.edu/data/amazon/): A dataset of product reviews and metadata from Amazon
+ Online advertising
    + [Criteo1TB](http://labs.criteo.com/2013/12/download-terabyte-click-logs-2/): A Terabyte display advertising dataset from Criteo
    + [Outbrain](https://www.kaggle.com/c/outbrain-click-prediction/data): A dataset of users' page views and clicks in Outbrain
+ Web search / sponsored search
    + [Yandex](https://www.kaggle.com/c/yandex-personalized-web-search-challenge): A click dataset for personalized Web search challenge from Yandex
    + [Tencent](https://www.kaggle.com/c/kddcup2012-track2): A click dataset for KDD Cup 2012 from Tencent
    + [Avito](https://www.kaggle.com/c/avito-context-ad-clicks/data): A dataset of contextual search ad clicks from Avito
+ CVR datasets
    + [YooChoose](https://2015.recsyschallenge.com/index.html): A sequence of click and purchase events in an e-commerce website from YooChoose
    + [Alimama](https://tianchi.aliyun.com/competition/introduction.htm?spm=5176.100069.5678.1.560d7a7eSjZLxq&raceId=231647): A dataset for sponsored product search in Alibaba
    + [JData](https://jdata.jd.com/html/detail.html?id=1): A dataset for purchase prediction in JD.com










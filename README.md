[![Documentation Status](https://readthedocs.org/projects/deepctr/badge/?version=latest)](https://deepctr.readthedocs.io/en/latest/?badge=latest)

# DeepCTR
A review and evaluation of CTR prediction models

### Models
| Model | Year | Reference | Status | 
| :-----: | :-------|:------------|:----------:|
| LR | |||
| FTLR ||||
| FM |2010 |[ICDM'10] [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)||
| FFM ||||
| GBDT ||||
| DNN ||||
| Wide&Deep ||||
| CCPM ||||
| FNN ||||
| PNN ||||
| DeepFM ||||
| NFM ||||
| AFM ||||
| xDeepFM |2018|[KDD'18] [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf), Microsoft||


### Datasets
| CTR Dataset | Description | #Instances | #Fields | #Train | #Validate | #Test | 
| :-----: |:------------|-----------:| -------:|-------:|----------:|------:|
| **Recommendation** |
| Taobao   | [A click dataset gathered from the recommender system in Taobao](https://tianchi.aliyun.com/datalab/dataSet.html?dataId=408) | | | | ||
| Outbrain  | [A dataset of users' page views and clicks in Outbrain](https://www.kaggle.com/c/outbrain-click-prediction/data) | | | | ||
| **Ad targeting** |
| Criteo  | [A Kaggle display advertising challenge dataset from Criteo](https://www.kaggle.com/c/criteo-display-ad-challenge/data) | | | | ||
| Avazo  | [11 days of click-through data from Avazu](https://www.kaggle.com/c/avazu-ctr-prediction/data) | | | | ||
| iPinyou  | [A real-time bidding algorithm competition dataset from iPinyou](http://contest.ipinyou.com/) | | | | ||

**Other relevant datasets:**
+ Ad targeting
    + [Criteo1TB](http://labs.criteo.com/2013/12/download-terabyte-click-logs-2/): A Terabyte display advertising dataset from Criteo
+ Web search / sponsored search
    + [Yandex](https://www.kaggle.com/c/yandex-personalized-web-search-challenge): A click dataset for personalized Web search challenge from Yandex
    + [Tencent](https://www.kaggle.com/c/kddcup2012-track2): A click dataset for KDD Cup 2012 from Tencent
    + [Avito](https://www.kaggle.com/c/avito-context-ad-clicks/data): A dataset of contextual search Ad clicks from Avito
+ CVR datasets
    + [YooChoose](https://2015.recsyschallenge.com/index.html): A sequence of click and purchase events in an e-commerce website from YooChoose
    + [Alimama](https://tianchi.aliyun.com/competition/introduction.htm?spm=5176.100069.5678.1.560d7a7eSjZLxq&raceId=231647): A dataset for sponsored product search in Alibaba
    + [JData](https://jdata.jd.com/html/detail.html?id=1): A dataset for purchase prediction in JD.com

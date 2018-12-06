[![Documentation Status](https://readthedocs.org/projects/deepctr/badge/?version=latest)](https://deepctr.readthedocs.io/en/latest/?badge=latest)

# DeepCTR
A review and evaluation of CTR prediction models

### Models
| Model | Year | Reference | Available | 
| :-----: | :-------|:------------|:----------:|
| LR | |||
| FTLR ||||
| FM |2010 |[ICDM'10] [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)||
| GBDT ||||
| CCPM |2015| [CIKM'15] [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676) | :heavy_multiplication_x: |
| FFM | 2016 | [RecSys'16] [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134), Criteo |:heavy_check_mark: |
| DNN | 2016 | [RecSys'16] [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf), Google |:heavy_check_mark: |
| Wide&Deep | 2016 | [DLRS'16] [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf), Google |:heavy_check_mark: |
| FNN |2016 | [ECIR'16] [Deep Learning over Multi-field Categorical Data: A Case Study on User Response Prediction](https://arxiv.org/abs/1601.02376), RayCloud |:heavy_check_mark: |
| PNN | 2016 | [ICDM'16] [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf) | :heavy_check_mark: |
| DeepFM | 2017 | [IJCAI'17] [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247), Huawei | :heavy_check_mark: |
| NFM |2017| [SIGIR'17] [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777) | :heavy_check_mark: |
| AFM |2017|[IJCAI'17] [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf) |:heavy_check_mark:|
| DCN | 2017 | [ADKDD'17] [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123), Google | :heavy_check_mark:|
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

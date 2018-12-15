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
| xDeepFM |2018|[KDD'18] [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf), Microsoft| :heavy_multiplication_x: |
| FWFMS | 2018 | [WWW'18] [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf), Oath, TouchPal, LinkedIn, Ablibaba | :heavy_multiplication_x: |


### Datasets
| Dataset |  #Fields | #Features | #Instances | #Training | #Validation | #Test | Positive Ratio |
| :-----: |:-----------:|:-----------:| :-------:|:-------:|:----------:|:------:|:------:|
| **Advertising** |
| [Criteo](https://github.com/anyai/deepCTR/tree/master/data#criteo)  |39 |  |45,840,617 |32,743,297 |6,548,660| 6,548,660||
| [Avazu](https://github.com/anyai/deepCTR/tree/master/data#avazu)  |  23 || 40,428,967 | 32,377,421 | 3,832,608 | 4,218,938 ||
| [iPinyou](https://github.com/anyai/deepCTR/tree/master/data#ipinyou)  | | | 14,759,750 |10,580,553 | 1,657,567 | 2,521,630 ||
| **Recommendation** |
| [Taobao](https://github.com/anyai/deepCTR/tree/master/data#taobao)   |  | | | ||||
| [Outbrain](https://github.com/anyai/deepCTR/tree/master/data#outbrain)  |  | | | ||||
| [Frappe](https://github.com/anyai/deepCTR/tree/master/data#frappe)  |  | | | ||||



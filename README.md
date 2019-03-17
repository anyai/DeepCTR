[![Documentation Status](https://readthedocs.org/projects/deepctr/badge/?version=latest)](https://deepctr.readthedocs.io/en/latest/?badge=latest)

# OpenCTR
Click-through rate (CTR) prediction is an important task in many industrial applications such as online advertising, recommender systems, and sponsored search. OpenCTR builds an open-source library for benchmarking existing CTR prediction models.

### Models
CTR prediction models currently available:

| Model | Conference | Paper | Available | 
| :-----: | -------: |:------------|:----------:|
| LR | WWW'07 |[Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) [**Microsoft**]| :heavy_check_mark: |
| FM |ICDM'10 | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)| :heavy_check_mark: |
| FTRL | KDD'13| [Ad Click Prediction: a View from the Trenches](https://www.researchgate.net/publication/262412214_Ad_click_prediction_a_view_from_the_trenches) [**Google**]||
| GBDT+LR |ADKDD'14| [Practical Lessons from Predicting Clicks on Ads at Facebook](https://dl.acm.org/citation.cfm?id=2648589) [**Facebook**] ||
| CCPM |CIKM'15| [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676) | :heavy_multiplication_x: |
| FFM | RecSys'16 | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) [**Criteo**] |:heavy_check_mark: |
| DNN | RecSys'16 | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) [**Google**] |:heavy_check_mark: |
| Wide&Deep | DLRS'16 | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) [**Google**] |:heavy_check_mark: |
| FNN |ECIR'16 | [Deep Learning over Multi-field Categorical Data: A Case Study on User Response Prediction](https://arxiv.org/abs/1601.02376) [**RayCloud**] |:heavy_check_mark: |
| PNN | ICDM'16 | [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf) | :heavy_check_mark: |
| DeepFM | IJCAI'17 | [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247), [**Huawei**] | :heavy_check_mark: |
| NFM |SIGIR'17| [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777) | :heavy_check_mark: |
| AFM |IJCAI'17| [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf) |:heavy_check_mark:|
| DCN | ADKDD'17 | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123) [**Google**] | :heavy_check_mark:|
| xDeepFM |KDD'18| [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) [**Microsoft**] | :heavy_multiplication_x: |
| FwFM | WWW'18 | [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) [**Oath, TouchPal, LinkedIn, Ablibaba**] | :heavy_multiplication_x: |

### Datasets
| Dataset |  #Fields | #Features | #Instances | #Train | #Test | Statistical CTR |
| :-----: |:-----------:|:-----------:| :-------:|:-------:|:----------:|:------:|:------:|
| [Criteo](./datasets#criteo)  | 39 |  | 45,840,617 | 39,798,482 | 6,042,135 | 25.62% |
| [Avazu](./datasets#avazu)  |  23 || 40,428,967 | 36,210,029 | 4,218,938 | 16.98% |
| [iPinyou](./datasets#ipinyou)  | | | 14,758,717 | 12,237,087 | 2,521,630 | 0.0726% |
| [Taobao](./datasets#taobao)   |  | | | |||
| [AliCCP](./datasets#aliccp)   |  | | | |||
| [Frappe](./datasets#frappe)  |  | | | |||



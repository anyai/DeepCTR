Introduction
===================================

DeepCTR aims to provide a set of open-source neural network wrappers 
implemented in Keras with tensorflow as backend that are popular in CTR 
prediction task. By using deepCTR, user just need to define their data loader 
function which returns formatted dataframe and some other information to 
build up their network. Then it can train on their own data with customizable 
parameters. The figure showing below illustrates the framework.

.. image:: WrapperFramework.png

The task of predicting click-through rate (CTR) is to estimate the probability 
a user will click on a recommended item (e.g. goods in e-commerce platform, 
advertisment in web site). The challenges of CTR prediction are:
                                         
- handling very high sparsity

  As there are a great number of users viewing a great number of items and 
  each impression log only associates with a single user and item. Thus the 
  data is very sparse and large scale.

- modeling feature interactions

  It is customizing to recommend those items with higher probability in 
  clicking for a target user. Therefore, modeling the interaction information 
  between item and user or other kinds of interaction is critical in CTR 
  prediction task.
  
For such high sparsity, the most direct way is applying a very simple linear 
model — Logistic Regression (LR), and cafefully adding handcrafted interaction
features to improve the capability of such simple linear model. Another brute
force approach is taking all interaction terms into model, which can also be 
implemented with Support Vector Machine (SVM) using polynomial kernel.

Obviously, these methods has serious limits:

- it requires expensive feature crafting effort

- it is unable to estimate reliable interaction weights

  As the weight w_ij for interaction pair (x_i, x_j) is updated only when x_i
  and x_j is nonzero. There is no doubt that (x_i, x_j) is more sparse 
  because both x_i and x_j have high sparsity.
GBDT+LR
===========

As mentioned in Introduction, the brute force approach modeling interaction
information is taking all interaction terms into consideration. Such brute way
is also applicable to high order interaction, thus supposing we just consider
the situaction no more than two order. 

Obviously, not all interaction terms are useful and it is critical to find out
those useful ones. Inspired by this, this hybrid model uses Gradient Boosting 
Decision Tree (GBDT) to get high order interaction feature. 

Concretely, the output of each individual tree is used to generate one
categorical feature with index of the leaf that instance falls in as value.
For example, consider the boosted tree model in figure shown below, which has
2 subtrees with 3 leafs and 2 leafs respectively. If an instance ends up in
leaf 2 and leaf 1 respectively, then the high order interaction feature vector
are [2,1] whose one-hot encoding vector is [0,1,0,1,0].

The hybrid model structure — concatenation of GBDT and LR is shown below.

.. image:: GBDT+LR.png
   :align: center
   :scale: 55 %
   

[**ACM'2014**]He, Xinran, et al. `Practical lessons from predicting clicks on ads at facebook <https://dl.acm.org/citation.cfm?id=2648589>`_, Proceedings of the Eighth International Workshop on Data Mining for Online Advertising. ACM, 2014.

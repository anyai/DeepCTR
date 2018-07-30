DCN (Deep & Cross Network)
===================================

The deep part of DCN is the same as FNN which embedding sparse feature 
into dense latent vector and apply DNN with concatenation of latent vectors as 
input. Simultaneously, DCN applys Cross Net to explicitly model both low-order 
feature interactions and high-order feature interactions. The cross operation
performs with formula::

  x_(l+1) = x_0 * (x_l)^T * w_l + b_l + x_l
  
Additionally, the term **`x_0 * (x_l)^T`** in Cross Net explicitly generates 
interactions but different from the term **`Σ_iΣ_j<v_i, v_j> * x_i * x_j`** in
FM. Specifically, the term **`x_0 * (x_l)^T`** generates element-level 
interaction while the term **`Σ_iΣ_j<v_i, v_j> * x_i * x_j`** is vector-level
interaction.

Its network structure is shown below.

.. image:: DCN.png
   :align: center
   :scale: 80 %

[**ADKDD'2017**]Wang, Ruoxi, et al. `Deep & cross network for ad click predictions <https://dl.acm.org/citation.cfm?id=3124754>`_, *Proceedings of the ADKDD'17*. ACM, 2017.
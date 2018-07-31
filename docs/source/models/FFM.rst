FFM (Field-aware Factorization Machines)
==========================================

**Model Equation**
  :math:`y(x):= bias + Σ_i(w_i * x_i) + Σ_iΣ_j<V_i[n], V_j[m]> * x_i^(m) * x_j^(n)`

FFM is based on the FM. FFM embeddings each category feature into multiple 
latent vectors (i.e. a latent vector matrix :math:`V_i`) and models those iteraction 
information between features as inner product of latent vectors from different 
field accordingly. Compared to FM, FFM has some advantages:

- it loses less information in modeling interation terms

  As introduced in FM, the latent vector of :math:`x_k` is shared in all iteraction 
  terms like (:math:`x_k`, :math:`x_j`). Therefore, the latent vector :math:`v_k`
  needs to cooperate with all of other vectors, which constrain :math:`v_k` 
  from better adapting to any :math:`v_j`. 
  
  With such idea, FFM clusters all feature into several fields and shares
  latent vector within each field respectively. All in all, it is a trade-off
  between capacity and reliability.
  
It can be implemented as neural network shown below.

.. image:: FFM.png
   :align: center
   :scale: 40 %

You can get the editable figure `here <https://www.processon.com/view/link/5b59addae4b08d3622916c48>`_.


[**ACM'2016**]Juan, Yuchin, et al. `Field-aware factorization machines for CTR prediction <https://dl.acm.org/citation.cfm?id=2959134>`_, Proceedings of the 10th ACM Conference on Recommender Systems. ACM, 2016.   

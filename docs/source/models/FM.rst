FM (Factorization Machines)
===================================

**Model Equation**
  :math:`y(x):= bias + Σ_i(w_i * x_i) + Σ_iΣ_j<v_i, v_j> * x_i * x_j`

FM is based on the idea of embedding which means that it treats each category 
feature as a latent vector and models those iteraction information as inner 
product of latent vectors. Thus FM has some advantages:

- it is able to model reliable interaction information

  For example, the latent vector of :math:`x_k` is invovled in all iteraction 
  terms like (:math:`x_k`, :math:`x_j`), thus the latent vector is estimated 
  well. With these informative latent vector :math:`v_i` and :math:`v_j`, FM 
  then model interaction terms as :math:`<v_i, v_j> * x_i * x_j`.

- it can handle such high sparisty and large scale data

  Though the number of term in FM is quadratic, the same feature :math:`x_i` 
  shares a single latent vector which makes it possible to be optimized into 
  linear complexity. Such optimization is based on the formula:
  
    :math:`2 * Σ_iΣ_j(x_i * x_j) = (Σ_ix_i)^2 - Σ_i(x_i)^2`
  
It can be implemented as neural network shown below.

.. image:: FM.png
   :align: center
   :scale: 40 %

You can get the editable figure `here <https://www.processon.com/view/link/5b5935e8e4b0be50eac1281c>`_.

[**ICDM'2010**]Rendle, Steffen. `Factorization machines <https://ieeexplore.ieee.org/abstract/document/5694074/>`_, *Data Mining (ICDM), 2010 IEEE 10th International Conference on*. IEEE, 2010.

DeepFM
===================================

The deep part of DeepFM is the same as FNN which embedding sparse feature 
into dense latent vector and apply DNN with concatenation of latent vectors as 
input. Simultaneously, DeepFM integrates FM with DNN which makes it model the
low-order feature interactions explicitly and high-order feature interactions
implicitly.

Its network structure is shown below.

.. image:: DeepFM_1.png
   :align: center
   :scale: 40 %

You can get the editable figure `here <https://www.processon.com/view/link/59c8dbfce4b0ef561374dea6>`_.

[**arXiv'2017**]Guo, Huifeng, et al. `Deepfm: a factorization-machine based neural network for ctr prediction <https://arxiv.org/abs/1703.04247>`_, *arXiv preprint arXiv:1703.04247* (2017).


# sa-nmt-en-vi
KeTran's sa-nmt on 2015 iwslt English-Vietnamese corpora and GPU training.

The model's source code is credited to the legend himself: https://github.com/ketranm/sa-nmt

Commands to train and perform translation are written in Google colab notebooks. The correct directory is as followed:

+sa-nmt-en-vi

+++++sa-nmt
+++++


To sucessfully run, some minor syntax changes must be taken care.

To train on GPU, TreeAttention constructor's orch.device must be changed from 'cpu' to 'cuda:0'


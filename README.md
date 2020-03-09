# sa-nmt-en-vi
KeTran's sa-nmt on 2015 iwslt English-Vietnamese corpora and GPU training.

The model's source code is credited to the legend himself: https://github.com/ketranm/sa-nmt

Commands to train and perform translation are written in Google colab notebooks. The correct directory is as followed:

--sa-nmt-en-vi

-----sa-nmt

--------iwslt

--------model.bpe

--------model.txt

--------model_best.pt

-----**[Google colab files]**


To sucessfully run, some minor syntax changes must be taken care.

To train on GPU, TreeAttention constructor's orch.device must be changed from 'cpu' to 'cuda:0'

Current model BLEUs are 23.36/24.61 (VI-EN) and 26.85/27.01 (EN-VI) compared to 2015 iwslt baselines. The breakdown of the author's model and example translated results can be found in **docs/**

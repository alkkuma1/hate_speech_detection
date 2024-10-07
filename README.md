# hate_speech_detection

This repository contains ny experiments in the space of hate speech analysis. I have used 3 datasets for my analysis:

## Dataset 1: Davidson's Dataset: https://www.kaggle.com/datasets/eldrich/hate-speech-offensive-tweets-by-davidson-et-al
## Dataset 2: Huggingface's measuring hate speech: https://huggingface.co/datasets/ucberkeley-dlab/measuring-hate-speech
## Dataset 3: HASOC's English dataset: https://hasocfire.github.io/hasoc/2020/files/English_2020.zip

The experiements are divided in 3 folders:
1. glove_embedding: The model is trained on a novel architecture using Glove embedding.
2. gte_large_en_v1.5: The model is trained on a above novel architecture using Alibaba's embedding.
3. RoBERTA: The datasets are finetuned on transformers and tested.

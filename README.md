# Hate Speech Detection

This repository contains my experiments in the space of hate speech analysis. I have used 3 datasets for my analysis:

- **Dataset 1**: Davidson's Dataset: [Davidson's Kaggle Dataset](https://www.kaggle.com/datasets/eldrich/hate-speech-offensive-tweets-by-davidson-et-al)
- **Dataset 2**: Huggingface's Measuring Hate Speech: [Huggingface Dataset](https://huggingface.co/datasets/ucberkeley-dlab/measuring-hate-speech)
- **Dataset 3**: HASOC's English dataset: [HASOC 2020 Dataset](https://hasocfire.github.io/hasoc/2020/files/English_2020.zip)

## Experiment Structure

The experiments are divided into 3 folders:

1. **glove_embedding**: The model in this folder is trained on a novel architecture using Glove embedding. The Glove embedding, a pre-trained word representation model, converts words into vectors that capture semantic meaning, which helps in identifying patterns and relationships in hate speech content. This model uses the Glove embeddings to represent words in a high-dimensional space, which improves the model's ability to detect hate speech by leveraging context and word relationships.
  
2. **gte_large_en_v1.5**: This folder contains a model trained using Alibaba's transformer-based embedding model. Alibaba’s `gte_large_en_v1.5` embedding is utilized to capture complex linguistic structures in the text, enhancing the model’s ability to understand nuanced language often found in hate speech. The embeddings are loaded via the Huggingface API, and the model architecture includes recurrent layers such as LSTM and GRU to handle the sequence-based nature of text data, allowing for improved classification of hate speech.

3. **RoBERTa**: In this folder, the datasets are fine-tuned using the RoBERTa transformer model. RoBERTa is a robustly optimized BERT pretraining approach that improves performance on downstream tasks like hate speech detection. The model architecture leverages the pre-trained RoBERTa model from Huggingface, which has been fine-tuned with the datasets mentioned above. This setup is designed to capture contextual information effectively, handling complex sentence structures and detecting hate speech more accurately. The tokenizer and configuration from Huggingface’s RoBERTa model are utilized for pre-processing and model setup.

Each folder contains the specific experiment's setup, data processing, and model training scripts. The RoBERTa experiments fine-tune the transformer model, leveraging its state-of-the-art performance in NLP tasks to detect hate speech with higher precision.

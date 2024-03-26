#### BERT-fine-tune-Humor-Detection

This project focuses on fine tuning BERT, a pre-trained transformer-based model, for humour detection.

To fine-tune the BERT model, the project utilizes a dataset of 200,000 short texts, 100k labelled as humorous and 100k as non-humorous. The dataset is taken from the paper _ColBERT: Using BERT Sentence Embedding in Parallel Neural Networks for Computational Humor_ (2022) by Issa Annamoradnejad and Gohar Zoghi https://paperswithcode.com/paper/colbert-using-bert-sentence-embedding-for


The dataset is preprocessed and split into train, validation, and test sets. To optimize model performance, training experiments are conducted with varying sample and batch sizes: samples of 500, 1000, 10k, 20k, 25k, 30k and 35k and batch number of 16 and 32.

Results show that increasing the number of samples improves accuracy up to a point, with smaller batch sizes outperforming larger ones. The project concludes that the model achieves a balance between underfitting and overfitting. However, limitations include hardware constraints and time-consuming fine-tuning processes. Overall, the project highlights the effectiveness of BERT for humour detection tasks while emphasizing the importance of training data size and batch size in model performance.

The model can be downloaded from here: https://huggingface.co/GeniaV/BERT_Humor_35k/tree/main


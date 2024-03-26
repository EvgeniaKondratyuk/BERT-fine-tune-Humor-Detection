#### BERT-fine-tune-Humor-Detection

This project focuses on fine-tuning BERT, a pre-trained transformer-based model, for humour detection.

To fine-tune the BERT model, the project utilizes a dataset of 200,000 short texts, 100k labelled as humorous and 100k as non-humorous. The dataset is taken from the paper _ColBERT: Using BERT Sentence Embedding in Parallel Neural Networks for Computational Humor_ (2022) by Issa Annamoradnejad and Gohar Zoghi https://paperswithcode.com/paper/colbert-using-bert-sentence-embedding-for

The dataset is preprocessed and split into train (80%), validation (10%), and test (10%) sets. To optimize model performance, training experiments are conducted with varying sample and batch sizes: 500, 1000, 10k, 20k, 25k, 30k, and 35k samples and batch numbers of 16 and 32.

The model's prediction accuracy score is 0.82 for the validation and 0.82 for the test sets.

Results show that increasing the number of samples improves accuracy up to a point, with smaller batch sizes outperforming larger ones. The project concludes that the model achieves a balance between underfitting and overfitting. However, limitations include hardware constraints and time-consuming fine-tuning processes. 
Overall, the project highlights the effectiveness of BERT for humour detection tasks while emphasizing the importance of training data size and batch size in model performance.

The experiment can be reproduced.

The repository contains the dataset in a CSV file, a folder with 2 codes for BERT fine-tuning, and the model application. Please make sure to download the model application before using it. The model is hosted here: https://huggingface.co/GeniaV/BERT_Humor_35k/tree/main.

##### Dependencies:

- python 3.6
- transformers package

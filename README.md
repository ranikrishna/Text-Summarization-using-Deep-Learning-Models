# Text-Summarization-using-Deep-Learning-Models

Abstract

Text Summarization, a vital aspect of natural language processing, aims to condense 
text while retaining its essential meaning. This process can be achieved through extractive and 
abstractive methods. Deep Learning faces challenges in this domain, including semantic 
understanding, preservation of meaning, efficient handling of long documents, and ensuring 
coherence and grammatical correctness. Despite these it offers advantages such as timesaving, 
facilitating information retrieval, scalability, and content personalization. Also, it faces the risk 
of losing important details, subjectivity in information selection, difficulty in handling complex 
texts, and variability in summary quality. Addressing these challenges remains an ongoing 
focus of research and development in the field of NLP. 

This paper proposes text summarization approach utilizing deep learning models, 
namely T5-base,T5-large,BART CNN, and PEGASUS. The methodology involves initial data 
cleaning and preprocessing of the dataset, followed by exploratory data analysis (EDA) to gain 
insights into the data. Subsequently, the Rouge scores and BLUE scores of each model are 
calculated to assess their summarization performance. After training the models, the Rouge and 
BLUE scores are re-evaluated to measure their effectiveness in generating summaries. The 
primary objective is to compare the performance of these models based on their Rouge scores, 
aiming to identify the model provides the highest Rouge score, indicative of better summary 
quality. This study contributes to the advancement of text summarization techniques and 
provides insights into the effectiveness of various deep learning models in this domain. 

Keywords: Text summarization, Deep learning, Abstractive text-summarization, EDA,  
model Evaluation, T5-base, T5-large,BART CNN-large, PEGASUS-large. 

Dataset--CNN/Daily-Mail News: 

The CNN/Daily-Mail dataset is sourced directly from the Hugging Face ‘datasets’ 
library. A well-known resource for building and evaluating text summarising models is the 
CNN/Daily Mail dataset. Since its initial introduction in 2015 by Karl Moritz Hermann and 
associates, it has established itself as a standard for evaluating summarization algorithms’ 
performance. This dataset is perfect for extractive and abstractive summarization models 
because it includes summaries of news stories from CNN and the Daily Mail. The dataset 
contains over 300,000 unique news articles.

Structure of the Dataset: 

The dataset is typically divided into three main CSV files: 

* train.csv 
There are approximately 287,113 articles and summaries. This split is used to train the 
summarization model, and it contains a bulk of data, which allows the model to learn 
the mapping from articles to summaries. 

* validation.csv 
There are approximately 13,368 articles and summaries. This split is used to validate 
the model during training. It helps in tuning hyperparameters and provides an unbiased 
evaluation to prevent overfitting. The performance tells us how well the model 
performs. 

* test.csv 
There are approximately 11,490 articles and summaries. This is used to evaluate the 
final performance of the trained model. It serves as the ultimate test to assess the 
model’s generalisation capability. 

Models Used 

In order to assess how well four cutting-edge deep learning models performed in 
producing acceptable and succinct summaries of a news dataset, we used them in this study. 
The models used were T5-base, T5-large, BART-CNN-large, and PEGASUS-large. Prior to 
delving into the detailed analysis of these models, we discuss the evaluation metrics used to 
identify the most effective model for text summarization. Specifically, we used ROUGE and 
BLEU scores as our primary metrics for performance assessment. These metrics and how we 
used them in our study are further examined in the sections that follow: 

1.ROUGE Score 
ROUGE (Recall-Oriented Understudy for Gisting Evaluation) scores are essential for 
assessing how effectively the text summarization algorithm works. These metrics serve as 
benchmarks for the quality of summarization algorithms by objectively measuring the degree 
to which machine-generated summaries align with human-written summaries. It ranges from 0 
to 1, and as the value of the rouge score is closer to 1, the model is more perfect and accurate. 
In the field of NLP and summarization, ROUGE scores are used to validate the efficacy of 
proposed methods, ensuring transparency and reproducibility of research findings. 

2.BLEU Score
Text summarization and machine translation systems are evaluated on their text quality 
using standards called BLEU (Bilingual Evaluation Understudy) scores. They evaluate the 
degree to which the generated text is comparable to reference texts, which are usually 
summaries or translations provided by humans. Although BLEU is more frequently linked to 
machine translation, text summarization also makes use of it. The scores range from 0 to 1, 
where 1 indicates a perfect match between the generated summary and the reference summary. 
However, achieving a score close to 1 is very rare. 

Conclusion

Results:  
A comparison chart that highlights each model’s ROUGE and BLEU scores provides a 
summary of the findings. On the CNN/Daily-Mail dataset, the model that performs the best for 
text summarization is the one with the highest scores. 

BART CNN-large is the best model for text summarization on the CNN/DailyMail dataset, 
regularly outperforming the other models in most measures, especially ROUGE-2, ROUGE
L, and BLEU scores. T5-large likewise performs well, particularly when it comes to ROUGE
1 scores. Although PEGASUS-large performs well in ROUGE-1, it falls short in other 
measures, indicating that it could use more adjustment and improvement. While it’s not the 
best, T5-base offers a reliable starting point for analysis. 
These insights give a clear picture of the advantages and disadvantages of each model, directing 
future developments and optimisations for text summarising jobs. 

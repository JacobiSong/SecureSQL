# SecureSQL 

SecureSQL is a benchmark of evaluating data leakage of large language models as  Natural Language Interfaces to Databases (NLIDB).

## 📄 Paper
Title: *SecureSQL: Evaluating Data Leakage of Large Language Models as  Natural Language Interfaces to Databases* 

Paper Link: https://aclanthology.org/2024.findings-emnlp.346/

## 📁 Dataset

This repository contains only one dataset, which merges selected portions of the Spider and Bird test sets into a security-focused benchmark. 

For complete details and methodology, please refer to the paper.

## 📦 Database

The benchmark database is composed of the Spider and Bird databases.

You can download the Spider and Bird databases separately and place their folders together.


## 🚀 Evaluation Metrics

We use the following metrics to evaluate secure SQL detection methods:

- **Accuracy**:  
  The proportion of correctly predicted queries (both safe and unsafe) out of all queries.  

- **Recall**:  
  The proportion of safe queries correctly identified as safe.  

- **Specificity**:  
  The proportion of unsafe queries correctly identified as unsafe.  

## 🧾 Citation

If you use this dataset in your research, please cite:
```
@inproceedings{song-etal-2024-securesql,
    title = "{S}ecure{SQL}: Evaluating Data Leakage of Large Language Models as Natural Language Interfaces to Databases",
    author = "Song, Yanqi  and
      Liu, Ruiheng  and
      Chen, Shu  and
      Ren, Qianhao  and
      Zhang, Yu  and
      Yu, Yongqi",
    editor = "Al-Onaizan, Yaser  and
      Bansal, Mohit  and
      Chen, Yun-Nung",
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2024",
    month = nov,
    year = "2024",
    address = "Miami, Florida, USA",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.findings-emnlp.346/",
    doi = "10.18653/v1/2024.findings-emnlp.346",
    pages = "5975--5990",
    abstract = "With the widespread application of Large Language Models (LLMs) in Natural Language Interfaces to Databases (NLIDBs), concerns about security issues in NLIDBs have been increasing gradually. However, research on sensitive data leakage in NLIDBs is relatively limited. Therefore, we propose a benchmark to assess the potential of language models to leak sensitive data when generating SQL queries. This benchmark covers 932 samples from 34 different domains, including medical, legal, financial, and political aspects. We evaluate 15 models from six LLM families, and the results show that the model with the best performance has an accuracy of 61.7{\%}, whereas humans achieve an accuracy of 94{\%}. Most models perform close to or even below the level of random selection. We also evaluate two common attack methods, namely prompt injection and inference attacks, as well as a defense method based on chain-of-thoughts (COT) prompting. Experimental results show that both attack methods significantly impact the model, while the defense method based on COT prompting dose not significantly improve accuracy, further highlighting the severity of sensitive data leakage issues in NLIDBs. We hope this research will draw more attention and further study from the researchers on this issue."
}
```


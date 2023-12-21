# Argument mining from Tweets related to COVID-19.
This repository contains baseline solutions of SMM4H'22 Task 2: Classification of stance and premise in tweets about health mandates (COVID-19).

<img width="1190" alt="smm4h_graphical_abstract" src="https://github.com/Veranchos/ArgMining_tweets/assets/37894718/44f183ea-b17c-4afc-a7b8-32b35a963c2c">

## Data 
[Data](data) directory contains:
- [Train](data/train) and [test](data/test/smm4h) data for SMM4H 2022 Task 2: tweets annotated for stance and premise prediction on three claims about COVID-19 mandates such as stay-at-home-orders, school closures, and face masks
- [2070](data/test/vaccine_tweets) annotated tweets about vaccine mandates, that were not used in the official SMM4H competition
- [600](data/test/vaccine_tweets/unused) annotated tweets about vaccine mandates with low inter-annotators agreement.

🤗 The dataset is also available at [Hugging Face](https://huggingface.co/datasets/veranchos/arg_mining_tweets).

## Models
Models that were used in comparison can be found in [models](models/) directory:
- [ROBERTA](models/ROBERTA_baseline)
- [COVID-Twitter-BERT](models/CT-Bert)
- [DAN-BERT](models/DAN-Bert)

## Citation
If you find our data and/or code useful, please cite:
```
@article{DAVYDOVA2024104555,
title = {Data and models for stance and premise detection in COVID-19 tweets: Insights from the Social Media Mining for Health (SMM4H) 2022 shared task},
journal = {Journal of Biomedical Informatics},
volume = {149},
pages = {104555},
year = {2024},
issn = {1532-0464},
doi = {https://doi.org/10.1016/j.jbi.2023.104555},
url = {https://www.sciencedirect.com/science/article/pii/S1532046423002769},
author = {Vera Davydova and Huabin Yang and Elena Tutubalina},
keywords = {Natural language processing, COVID-19 tweets, Opinion mining, Argument mining, Stance detection, Premise detection},
abstract = {The COVID-19 pandemic has sparked numerous discussions on social media platforms, with users sharing their views on topics such as mask-wearing and vaccination. To facilitate the evaluation of neural models for stance detection and premise classification, we organized the Social Media Mining for Health (SMM4H) 2022 Shared Task 2. This competition utilized manually annotated posts on three COVID-19-related topics: school closures, stay-at-home orders, and wearing masks. In this paper, we extend the previous work and present newly collected data on vaccination from Twitter to assess the performance of models on a different topic. To enhance the accuracy and effectiveness of our evaluation, we employed various strategies to aggregate tweet texts with claims, including models with feature-level (early) fusion and dual-view architectures from the SMM4H 2022 Task 2 leaderboard. Our primary objective was to create a valuable dataset and perform an extensive experimental evaluation to support future research in argument mining in the health domain.}
}
```

# Argument mining from Tweets related to COVID-19.
This repository contains baseline solutions of SMM4H'22 Task 2: Classification of stance and premise in tweets about health mandates (COVID-19).

<img width="1190" alt="smm4h_graphical_abstract" src="https://github.com/Veranchos/ArgMining_tweets/assets/37894718/44f183ea-b17c-4afc-a7b8-32b35a963c2c">

## Data 
[Data](data) directory contains:
- [Train](data/train) and [test](data/test/smm4h) data for SMM4H 2022 Task 2: tweets annotated for stance and premise prediction on three claims about COVID-19 mandates such as stay-at-home-orders, school closures, and face masks
- [2070](data/test/vaccine_tweets) annotated tweets about vaccine mandates, that were not used in the official SMM4H competition
- [600](data/test/vaccine_tweets/unused) annotated tweets about vaccine mandates with low inter-annotators agreement.

  The dataset is also available at 🤗[Hugging Face](https://huggingface.co/datasets/veranchos/arg_mining_tweets).

## Models
Models that were used in comparison can be found in [models](models/) directory:
- [ROBERTA](models/ROBERTA_baseline)
- [COVID-Twitter-BERT](models/CT-Bert)
- [DAN-BERT](models/DAN-Bert)

## Citation
If you find our data and/or code useful, please cite:
```
@inproceedings{davydova-tutubalina-2022-smm4h,
    title = "{SMM}4{H} 2022 Task 2: Dataset for stance and premise detection in tweets about health mandates related to {COVID}-19",
    author = "Davydova, Vera  and
      Tutubalina, Elena",
    booktitle = "Proceedings of The Seventh Workshop on Social Media Mining for Health Applications, Workshop {\&} Shared Task",
    month = oct,
    year = "2022",
    address = "Gyeongju, Republic of Korea",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.smm4h-1.53",
    pages = "216--220",
    abstract = "This paper is an organizers{'} report of the competition on argument mining systems dealing with English tweets about COVID-19 health mandates. This competition was held within the framework of the SMM4H 2022 shared tasks. During the competition, the participants were offered two subtasks: stance detection and premise classification. We present a manually annotated corpus containing 6,156 short posts from Twitter on three topics related to the COVID-19 pandemic: school closures, stay-at-home orders, and wearing masks. We hope the prepared dataset will support further research on argument mining in the health field.",
}
```

# Argument mining from Tweets related to COVID-19.
This repository contains baseline solutions of SMM4H'22 Task 2: Classification of stance and premise in tweets about health mandates (COVID-19).

<img width="1190" alt="smm4h_graphical_abstract" src="https://github.com/Veranchos/ArgMining_tweets/assets/37894718/44f183ea-b17c-4afc-a7b8-32b35a963c2c">

## Data 
[Data](data) directory contains:
- [Train](data/train) and [test](data/test/smm4h) data for SMM4H 2022 Task 2: tweets annotated for stance and premise prediction on three claims about COVID-19 mandates such as stay-at-home-orders, school closures, and face masks
- [2070](data/test/vaccine_tweets) annotated tweets about vaccine mandates, that were not used in the official SMM4H competition
- [600](data/test/vaccine_tweets/unused) annotated tweets about vaccine mandates with low inter-annotators agreement.

## Models
Models that were used in comparison can be found in [models](models/) directory:
- [ROBERTA](models/ROBERTA_baseline)
- [COVID-Twitter-BERT](models/CT-Bert)
- [DAN-BERT](models/DAN-Bert)


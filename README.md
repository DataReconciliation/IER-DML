# Datasets for IER-DML paper
## Datasets Overview  
This document provides an overview of the datasets designed for the IER-DML project. These datasets aim to address the challenges of incrementally resolving and disambiguating entity descriptions in dynamic environments. We have adopted and extended benchmark datasets provided by [DeepMatcher](https://github.com/anhaidgroup/deepmatcher), covering various domains such as products, citations, and restaurant names. Each dataset consists of entities originating from two associated relational tables, with each entity possessing multiple attributes. 
## Dataset Information
This study uses four authoritative ER benchmark datasets, all sourced from the ER-Benchmark and Magellan repositories.

| Dataset            | Domain     | \|D1\| | \|D2\| | #Matches | #Attr |
| ------------------ | ---------- | ------ | ------ | -------- | ----- |
| Amazon-Google (AG) | software   | 1363   | 3226   | 11460    | 1300     | 3     |
| DBLP-Scholar (DS)  | citation   | 2616   | 64263  | 5347     | 4     |
| DBLP-ACM (DA)      | citation   | 2616   | 2294   | 2224     | 4     |
| Fodors-Zagats (FZ) | restaurant | 532    | 330    | 946      | 110      | 6     |

Notices:

- After removing the initial training set, the remaining data are divided into 5–9 time steps (depending on the dataset size).
- The datasets in each time step are mutually disjoint to simulate the injection of new data in real dynamic scenarios.

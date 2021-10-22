# Continual Few-Shot Learning for Text Classification (EMNLP 2021)

## Overview
This repository contains the datasets that we curated as a benchmark for Continual Few-Shot Learning (CFL) task. In CFL task, a system is challenged with a difficult phenomenon and asked to learn to correct mistakes with only a few (10 to 15) training examples.

## Datasets Format
You can download the datasets from [here]().

In our CFL framework we consider two scenarios: (1) few-shot learning setup; (2) continual few-shot learning setup. In each setup, we have 5 and 2 categories for SNLI and IMDB datasets, respectively. For few-shot learning setup, each category has 3 train sets. Below is an overview of the directory structure.

    .
    ├── few_shot                   
    │   ├── SNLI        
    │   │    ├── change-action-1
    │   │    │    ├── (train/dev/test).tsv
    │   │    ├── change-action-2
    │   │    │    ├── (train/dev/test).tsv
    │   │    ├── change-action-3
    │   │    │    ├── (train/dev/test).tsv
    │   ├── IMDB
    │   │    ├── ...
    ├── continual
    │   ├── SNLI        
    │   │    ├── change-action
    │   │    │    ├── (train/dev/test).tsv
    └── ...

### Categories

Dataset  | Categories
---------| -------------------------------
SNLI     | Insert/remove phrases, Substitute entities,<br> Substitute evidence, Modify entity details, <br> and Change action
IMDB     | Modifiers and Negation


## Reference

If you find this code helpful, please consider citing the following paper:

    @inproceedings{pasunuru2021continual,
        title={Continual Few-Shot Learning for Text Classification},
        author={Pasunuru, Ramakanth and Stoyanov, Veselin and Bansal, Mohit},
        booktitle={EMNLP},
        year={2021}
    }

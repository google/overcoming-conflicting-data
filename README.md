# Conflicting Data for Model Updates

This repository contains the synthetic data for the paper:  [Overcoming Conflicting Data when Updating a Neural Semantic Parser](https://arxiv.org/pdf/2010.12675.pdf), which was presented at the Workshop on NLP for Conversational AI (NLP4ConvAI) at EMNLP 2021.

The data is derived from, and presented in the same format as the data in:  [Semantic Parsing for Task Oriented Dialog using Hierarchical Representations](https://research.fb.com/publications/semantic-parsing-for-task-oriented-dialog-using-hierarchical-representations/)

## Data

The generated data is present in the `top_data/remodeling` directory.  Each of the 5 synthesized updates are in a separate subfolder of this directory, and each update folder is broken down into the V1, V2, and evaluation data for that update.  All experiments in the paper are done on a targeted evaluation split specific to each update, which is stored in the `devset` folders in this repository.  The original TOP testset is included in the `testset` folders, but was not used for numbers reported in the paper.  Note that within the `V1_trainset` partitions, the data in the `changed_relabeled` folders represent "oracle" labels after the update and should not be used for training models.

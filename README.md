# BERT Fine-Tuning and Reproduction

CS-320 Artificial Neural Networks & Deep Learning semester project (Fall 2026), NUST. Group G03. Paper P09: BERT.

We rebuild the BERT paper in PyTorch, reproduce its SST-2 fine-tuning result at Colab scale, run the same model on a second dataset the paper did not use, and study it with one-factor-at-a-time ablations. We also write the core BERT encoder ourselves and check it against the HuggingFace implementation.

## Team

- Areeba Zahra (Team Lead)
- Madeeha Noor
- Qudsia Batool

## Paper

Devlin, J., Chang, M.-W., Lee, K., Toutanova, K. (2019). BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding. NAACL. https://arxiv.org/abs/1810.04805

## What this project does

1. Reproduce: BERT-base fine-tuned on SST-2 (paper reports 93.5%; we aim for about 92% on the validation set).
2. New dataset: IMDB (and/or AG News) with a TF-IDF + Logistic Regression baseline.
3. Ablations: learning rate, batch size, epochs, maximum length, [CLS] vs mean pooling, frozen layers.
4. Beyond the lecture: our own BERT encoder, loaded with pretrained weights and matched to the library output.
5. Gradio demo.

## Data

- SST-2 (GLUE). Socher et al. (2013); Wang et al. (2019). Licence: to be filled in.
- IMDB. Maas et al. (2011). Licence: to be filled in.

## Run the notebook

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/madeeha-noor/BERT-Fine-Tuning-Reproduction/blob/main/notebooks/bert_project.ipynb)

Use a T4 GPU runtime. Install dependencies with `pip install -r requirements.txt`. Checkpoints are saved to Google Drive and are not stored in this repository.

## Repository

- `proposal/` project proposal
- `notebooks/` Colab notebook (reproduction, new dataset, ablations, debugging)
- `CONTRIBUTIONS.md` who did what

## Results

To be added as the milestones are completed.

## AI assistance

An AI assistant was used for project planning and for the initial file templates. Implementation, experiments and analysis are done by the team.

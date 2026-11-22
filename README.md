# Protein Secondary Structure Prediction

## Overview

This project predicts the secondary structure of proteins from amino acid sequences. Embeddings from the pretrained Evolutionary Scale Modeling (ESM) protein language model were used as features to train a Random Forest classifier to evaluate how well these embeddings capture structural information.

## Data

The dataset is not included in this repository.

The code expects a `train.tsv` with the following columns:

| Column     | Description                              |
|------------|------------------------------------------|
| `id` | Amino acid sequence (string)             |
| `secondary_structure`    | Secondary structure class (one of 9)     |

The ID contains a three-letter abbreviation for the amino acid and the position of the amino acid within the protein.

The 9 classes are labeled based on secondary structure categories (ie. alpha-helix, residue in isolated beta-bridge, etc.)

## Project Recognition
This project was completed by Jenna Jabourian, as part of the course **COM SCI CM121: Probabilistic Models in Computational Genomics** course at UCLA. 

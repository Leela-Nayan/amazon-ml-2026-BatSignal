# Business Entity Resolution — Amazon ML Challenge 2026

## Setup
pip install -r requirements.txt

## Run order
1. src/normalization.py — clean/canonicalize name+address fields
2. src/blocking.py       — generate candidate_pairs.tsv
3. src/features.py       — build the feature matrix for candidate pairs
4. src/train.py          — train the pairwise classifier
5. src/infer.py          — score test candidates, apply threshold, write matching_results.tsv
6. src/metric.py         — F_0.5 scorer, validated against the challenge's worked example

## Reproduce end-to-end
(fill in exact commands once the pipeline runs)

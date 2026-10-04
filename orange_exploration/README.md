# Preliminary Orange Exploration

Shamma Alalawi created these Orange workflows during the initial exploration of the PhiUSIIL phishing dataset.

## Files

- `PhiUSIIL_Main_Experiment.ows`: initial comparison of logistic regression, random forest, SVM, gradient boosting, and a neural network.
- `PhiUSIIL_Ablation_Without_URLSimilarityIndex.ows`: exploratory experiment removing URLSimilarityIndex.
- `PhiUSIIL_Model_Size.ows`: workflow for training and saving Orange models for file-size inspection.

## Relationship to the final experiments

These workflows document the preliminary exploration. The final assignment results come from the Google Colab notebook in the repository root.

The Colab experiments use URL deduplication, domain-disjoint training/validation/test partitions, and a shared preprocessing protocol. Orange and Colab results should not be combined into one comparison because their experimental settings differ.

## Opening the workflows

Open the `.ows` files in Orange Data Mining. The File widget may reference a local dataset path; select your downloaded PhiUSIIL dataset before running the workflow. Check the widget settings and input columns before execution.

Dataset source:
https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset

Dataset licence: CC BY 4.0.

## Saved model files

The large `.pkcls` files are not included here. Inspection showed that they contain stored data alongside the fitted models, so their total file sizes are not directly comparable with the serialized Colab pipeline sizes.

## Contribution

Orange workflow development and preliminary experiments: Shamma Alalawi.

The workflows were uploaded to this repository by Meera Alalawi.

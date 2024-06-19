# PosthocXAI4BCI
Code for the paper "Towards Optimising EEG Decoding using Post-hoc Explanations and Domain Knowledge", EMBC 2024

# Installing dependencies
Use requirements.txt with Python 3.7 or higher

# Reproducing results
Dataset: To skip the pre-processing step to generate epoch data, you may refer to this [repo](https://github.com/xiangzhang1015/Deep-Learning-for-BCI) for the dataset.

To use Conformer architecture with 3 conditions:
1. Train the model using all channel data
2. Using MI relevant data
3. Using feature relevance
refer to the file Conformer_top_16_subs.ipynb. Change the class EEGMMIDTrSet and EEGMMIDTsSet to ensure the correct choice of channels.

extractResults.ipynb helps extract the model performance and save the results in .csv format

Notebooks GradCAM_MIchannels.ipynb helps generate feature relevance explanations in the form of topomaps and TF plots as visualised in the paper.

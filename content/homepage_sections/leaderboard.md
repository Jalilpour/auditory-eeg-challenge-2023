---
title: "Get started"
weight: 40
description: "Get started"
---
## Get started

1) Send a mail to [auditoryeegchallenge@kuleuven.be](auditoryeegchallenge@kuleuven.be) with the names of the team members, emails, and affiliations. You will receive a password to download the data  
2) Download the data from [https://rdr.kuleuven.be/dataset.xhtml?persistentId=doi:10.48804/K3VSND](our official repository) or get the already zipped files from  [ICASSP-2023-eeg-decoding-challenge-dataset](https://kuleuven-my.sharepoint.com/:f:/g/personal/lies_bollens_kuleuven_be/EkaIjOmoPIRHmYLdLK8b2VQBY_2ouqNSnHHTHyRl3Zn-2w?e=KhX7d0)
   - **split_data(.zip)** contains already preprocessed, split and normalized data; ready for model training/evaluation. If you want to get started quickly, you can opt to only download this folder/zipfile.
   - **preprocessed_eeg(.zip)** and **preprocessed_stimuli(.zip)** contain preprocessed EEG and stimuli files ( speech envelope and mel spectrogram features) respectively. At this stage data is not yet split into different sets and not normalized. To go from this to the data in **split_data.zip**, you will have to run _task*/create_data/split_and_normalize.py_ for the task you want to work on.
   - **raw_eeg(_x.zip)** and **stimuli(.zip)** contain the raw EEG and stimuli files. If you want to process the stimuli files, you can run _task*/create_data/speech_features.py_. Speech Envelope and/or mel spectrogram features will be stored in the processed_stimuli. Currently, no preprocessing code is made available to preprocess EEG, so you will have to write your own implementation or use the precomputed processed_eeg folder.

For more details concerning the dataset, we refer to [the dataset paper](https://www.biorxiv.org/content/10.1101/2023.07.24.550310v1). 

3) Clone the starting code from our [github repository](https://github.com/exporl/auditory-eeg-challenge-2023-code) and get started. 
The repository contains preprocessing code, as well as baseline models for each of the tasks. 

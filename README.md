# EE495 Final Project  
Scientific Machine Learning for Spike Detection and Classification in Neural Electrophysiology Data

## Project description

This project develops a machine learning pipeline for spike detection and classification
in neural electrophysiology recordings.

The goal is to improve traditional spike sorting methods by combining
signal processing, clustering, and convolutional neural networks (CNN).

This project is based on neural recording data from bioelectronic experiments
using multi-channel neural interface devices.

The pipeline includes:

- Band-pass filtering
- Spike detection using adaptive threshold
- Dimensionality reduction with UMAP
- Clustering with DBSCAN
- CNN-based spike classification

This approach provides a more robust and automated method for spike sorting,
especially in noisy recordings.


## Repository structure

notebooks/  
Contains all Jupyter notebooks used in this project

report/  
2-page final report (PDF)

slides/  
Presentation slides and video link

results/  
Example outputs

requirements.txt  
Python dependencies


## How to run

Install dependencies: pip install numpy scipy umap-learn scikit-learn torch

Run notebooks in order:

1_RawProcessing  
2_SpikeSorting_CNN_Pipeline  
3_train_spike_cnn


## Machine learning part

The machine learning component uses a 1D convolutional neural network
to classify spike waveforms obtained from clustering.

The model supports incremental learning and can be updated when new spike classes appear.


## Presentation video

Link:
https://docs.google.com/presentation/d/1stI0OSZP8kjo3vhBuuX4afTxFNyo4qBn/edit?usp=share_link&ouid=114509514834407904065&rtpof=true&sd=true
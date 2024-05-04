# Reproduction of Results published in 'Predicting intraoperative hypotension using deep learning with waveforms of arterial blood pressure, electroencephalogram, and electrocardiogram: Retrospective study' 

This repository retains code attempting to replicate the findings described in Yo, Jang, Kwon, Lee, Jung, Byun, Jeong: ‘Predicting intraoperative hypotension using deep learning with waveforms of arterial blood pressure, electroencephalogram, and electrocardiogram: Retrospective study’ Plos One. https://doi.org/10.1371/journal.pone.0272055

## Dataset

The dataset used is open access: https://osf.io/dtc45/. It can be obtained after signing the Data Use Agreement (https://vitaldb.net/docs/?documentId=1OyhiDYbN-VJ6TOme-Fkj4wbqJkVT3UazELcbCXcHmiY)

** The currently available dataset includes intraoperative recordings from 6,388 patients (https://vitaldb.net/dataset/). Interstingly, the original paper included 39,600 cases in the Vital DB. I am not sure whether the databse has been updated or whether the authors had access to additional cases. For this analysis, the currently available 6,388 patients will be included **

## Load Dataset

1) Download the .vital files after signing the Data Use Agreement (each .vital file corresponds to the tracings of one patient during surgery)
2) Update the directory indicating where the .vital files are stored ('raw_data_dir' in the notebook)

## Data Preprocessing

Data processing contains the follwing steps:
1) Identification of cases and controls (each patient can contribute multiple cases and controls)
2) Preprocessing including filtering and normalizing
3) Splitting into train / val / test sets (given the smaller dataset compared to the original publication, a 70:10:20 split is used)

## Trained Models

Model checkpoints have been created and are available in the repository. Make sure to save those in the same directory with the notebook or to update the directory.









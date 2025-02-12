# HMS - Harmful Brain Activity Classification  

This repository contains the code for the **HMS - Harmful Brain Activity Classification Kaggle Competition**, where we developed deep learning models to **detect and classify seizures and other harmful brain activity** using **electroencephalography (EEG) signals** and their corresponding **spectrograms** recorded from critically ill hospital patients.  

This competition was part of the course **Machine Learning in Practice (NWI-IMC030)**, where we worked in teams of three to compete. More details about the competition can be found on the [Kaggle competition page](https://www.kaggle.com/competitions/hms-harmful-brain-activity-classification).  

## Models  

This repository contains **three** models we developed for EEG classification:  

1. **EEGNet** – A hybrid model combining a **convolutional pathway** and a **Gated Recurrent Unit (GRU) pathway** to classify EEG signals.  
![image](EEGNet.png)  

2. **EEGNet Parallel** – A variation of EEGNet where each temporal chain is processed in **parallel** before concatenation.  
![image](EEGNetParallel.png)  

3. **Ensemble Model** – Our final submission used an **ensemble** combining:
   - EEGNet  
   - EEGNet Parallel  
   - WaveNet (pre-trained)  
   - EfficientNetB0 (pre-trained, trained on spectrograms)  

   *(Note: The WaveNet and EfficientNetB0 models were not developed by us, but were included in our final submission.)*  

Each notebook details the **data preprocessing, model training, and inference process**. The attached **report** provides further details about the models and an overview of the competition.  

## Installation  

These notebooks are designed to run in the **Kaggle environment** dedicated to this competition. To run the notebooks, follow these steps:

1. **Download the competition data** from the [Kaggle page](https://www.kaggle.com/competitions hms-harmful-brain-activity-classification).  
2. **Upload the notebooks** to the Kaggle environment.  
3. **Run the notebooks**—no additional installation is required.  

**Note:** Training and inference are handled in separate notebooks. Be sure to follow the provided instructions in each notebook.  
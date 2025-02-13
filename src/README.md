# Sleep Apnea ECG Classifier

This project aims to classify sleep apnea events using ECG data. The dataset is from the **Apnea-ECG Database**, and the goal is to process the ECG data, extract features (like spectrograms), and use a deep learning model for classification.

## About the Apnea-ECG Dataset

The **Apnea-ECG Database** is a collection of ECG signals specifically collected to study the presence of sleep apnea. Sleep apnea is a sleep disorder characterized by interruptions in breathing during sleep, and it can be detected through changes in the ECG signal. The dataset contains both normal and apnea events labeled in the annotations.

- **ECG signals**: Each file contains ECG data sampled at 100 Hz.
- **Annotations**: Each event is labeled as either 'A' for apnea or 'N' for normal breathing, where the apnea events represent moments of interrupted breathing, and normal breathing events represent stable sleep patterns.
  
In this project, we will use the ECG signals from the dataset to train a machine learning model capable of identifying sleep apnea events based on the ECG features. We will process the signals into spectrograms, which are a visual representation of the frequency content of the signal over time, to be used as input for the model.


## Setting Up The Environment

To set up the environment for this project, follow these steps:

### 1. Clone the repository

Clone the repository to your local machine:

```bash
git clone https://github.com/josephgawler/SleepApneaClassifier
cd sleep-apnea-ecg-classifier
```

### 2. Create Virtual Environment

```bash
# Create a virtual environment
python3 -m venv env
```

```bash
# Activate the virtual environment
# On Windows:
env\Scripts\activate
# On macOS/Linux:
source env/bin/activate

# Install all necessary dependencies
pip install -r requirements.txt
```


### 3. Placement of Dataset

Download the [dataset](https://www.physionet.org/content/apnea-ecg/1.0.0/) from here. Once downloaded, extract the dataset and place the files in the data/ folder. Your directory should look something like this:

```
src/
│
├── data/
│   └── apnea-ecg-database-1.0.0/
│       ├── a01.dat
│       ├── a01.hea
│       └── a01.apn
└── ...
```


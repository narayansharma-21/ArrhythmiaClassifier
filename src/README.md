# Sleep Apnea ECG Classifier

This project aims to classify differnet types of heartbeats from ECG signals using CNNs. We aim to identify and classify various arrhythmias using the **MIT-BIH Arrhythmia Database**.

## Dataset

The **MIT-BIH Arrhythmia Database** contains 48 half-hour excerpts of two-channel ambulatory ECG recordings, obtained from 47 subjects studied by the BIH Arrhythmia Laboratory between 1975 and 1979. 

The dataset includes annotations for each heartbeat, indicating the type of arrhythmia.

**Classes:**
Normal beat (N)
Left bundle branch block beat (L)
Right bundle branch block beat (R)
Atrial premature beat (A)
Ventricular premature contraction (V)
Fusion of ventricular and normal beat (F)
Unclassifiable beat (Q)
Other types of beats as specified in the dataset

**Generating Spectrograms**: We convert the one-dimensional ECG signals into two-dimensional spectrograms. This helps in capturing the time-frequency characteristics of the signals.


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


### 3. Prepare the data

Download the [dataset](https://physionet.org/content/mitdb/1.0.0/) from here. Once downloaded, extract the dataset and place the files in the data/ folder. Your directory should look something like this:

```
src/
│
├── data/
│   └── mit-bih-arrhythmia-database-1.0.0
│       ├── 100.atr
│       ├── 100.dat
│       └── 100.hea
└── ...
```


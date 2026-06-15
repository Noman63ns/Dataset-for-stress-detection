# Multimodal Non-Invasive Physiological Signal Dataset

This dataset contains non-invasive physiological signals (ECG, EEG, and PPG) collected from 32 participants across three distinct cognitive states: rest, stress induced by calculation tasks, and stress induced by identification tasks.

## Directory Structure

```text
├── brain_performance/
│   ├── identification_performance.csv
│   
└── raw_data/
    ├── s1/
    │   ├── s1 all.csv
    │   ├── s1 all stress.csv
    │   └── s1 all flowers.csv
    ├── s2/
    │   ├── s2 all.csv
    │   ├── s2 all stress.csv
    │   └── s2 all flowers.csv
    └── ... (up to s32)
```

## Dataset Description

### 1. Brain Performance (`/brain_performance`)
This folder contains behavioral metrics and task performance data. 
* **`identification_performance.csv`**: Tracks participant performance during the identification stress task. It records the total number of samples presented to each participant, along with the count of correct and incorrect answers.

### 2. Raw Data (`/raw_data`)
This folder contains the authentic, unprocessed physiological signal data. It is divided into 32 subfolders labeled `s1` through `s32`, where each folder represents a unique subject (Sample 1, Sample 2, etc.).

Each sample folder contains exactly three signals data:
* **`ecg`**: Electrocardiogram signal data capturing cardiac activity.
* **`eeg`**: Electroencephalogram signal data capturing brainwave activity.
* **`ppg`**: Photoplethysmogram signal data capturing peripheral blood volume pulse.

## Experimental States
The signals in the raw data files span three specific experimental phases:
1. **Rest**: Baseline state with no cognitive load.
2. **Stress on Calculation**: Stress induced by mental arithmetic tasks.
3. **Stress on Identification**: Stress induced by visual or cognitive identification tasks (performance recorded in the `brain_performance` folder).

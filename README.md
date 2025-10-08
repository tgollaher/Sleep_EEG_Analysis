# Sleep EEG Amplitude Analysis (MNE-Python)

## Project Goal
This project demonstrates the fundamental difference in brainwave amplitude (voltage) across the main human sleep stages (N1, N2, N3, REM, Wake) using standard neurophysiological analysis techniques in Python.

## Scientific Principle Demonstrated
The analysis confirms that **Deep Sleep (N3)** is characterized by high-amplitude, low-frequency **Delta waves**, resulting in the largest overall average voltage of all stages. This demonstrates cortical synchronization during deep sleep.

##️ Technology and Libraries
* **Language:** Python
* **Core Library:** **MNE-Python** (used for data handling, epoching, and Evoked Potential calculation)
* **Data Source:** **Sleep-EDF Expanded Dataset** (publicly available via PhysioNet). The data is organized according to the **Brain Imaging Data Structure (BIDS)** standard.

## Key Analytical Steps Performed

1.  **Data Loading:** Loaded raw Polysomnography (PSG) data in the EDF format and imported the manual hypnogram annotations (sleep staging).
2.  **Epoching:** Segmented the continuous EEG data into 30-second epochs, labeling each epoch with its corresponding sleep stage (N1, N2, N3, REM, Wake).
3.  **Evoked Potential Calculation:** Calculated the **Evoked Potential** (the average EEG waveform for each specific sleep stage) using the MNE `.average()` method.
4.  **Visualization:** Plotted the five averaged waveforms simultaneously for visual comparison.

## Key Finding
The **N3 (Deep Sleep)** stage exhibited the highest average amplitude ($\mu V$) compared to all other stages, successfully validating a core neurophysiological principle.

---

## Data Citation and Acknowledgment

This analysis was performed using publicly available data from the **OpenNeuro** database.

**The full data citation can be found in the original file:** `README_DATASET_SOURCE.md`

We thank the original researchers for making this data available under the terms of the CC0 license.

---

## Code File
* **Code:** `Sleep_EEG_Amplitude_Analysis.ipynb` (Jupyter Notebook containing all processing steps and visualization

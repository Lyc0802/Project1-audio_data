# Dataset Documentation

## 1. Overview
This dataset consists of **4 different musical instruments**, each with **600 WAV files**, totaling **2400 audio samples**. The instruments included are:

- **Bass**  
- **Drum**  
- **Guitar**  
- **Piano**  

This dataset is intended for **audio classification** and **instrument recognition** tasks.

## 2. Data Type
- **Format**: WAV  
- **Sampling Rate**: unknown
- **Bit Depth**: 64bit
- **Duration**: 3sec~10min
- **Channels**: Mono

## 3. Data Source
- **External Source**: This dataset was collected from [Freesound](https://freesound.org/) using the Freesound API. Freesound is an online collaborative database of Creative Commons licensed audio samples. Each audio file was retrieved based on instrument-related keywords such as "bass", "drum", "guitar", and "piano".  
- **Self-Collected**: N/A (All data was obtained from an external source).   

## 4. Data Composition
- **Total Samples**: 2400  
- **Per Instrument**: 600 samples  

## 5. Data Collection Conditions
- **File Naming Convention**: {instrument_label}_001.wav

## 6. Data Collection Process

- **Hardware Used**: N/A (Audio files were collected from an online source, Freesound, rather than recorded manually).  

- **Software Used**:  
  - **Freesound API**: Used to query and download audio samples based on instrument-related keywords.  
  - **Python Libraries**:  
    - `requests` – For making API requests to Freesound.  
    - `librosa` – For audio analysis and feature extraction.  
    - `soundfile` – For reading and writing WAV files.  
    - `pydub` – For audio trimming and conversion when needed.  

## 7. Sample Data
Example file structure:
```
       audio_data/
       ├── bass/
       │   ├── bass_001.wav
       │   ├── bass_002.wav
       │   └── ...
       ├── drum/
       │   ├── drum_001.wav
       │   ├── drum_002.wav
       │   └── ...
       ├── guitar/
       │   ├── guitar_001.wav
       │   ├── guitar_002.wav
       │   └── ...
       ├── piano/
       │   ├── piano_001.wav
       │   ├── piano_002.wav
       │   └── ...
```


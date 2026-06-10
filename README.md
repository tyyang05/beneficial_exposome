# Beneficial Exposome Wearables Analysis

This repository contains the code used to analyze the wearable physiology arm of the Beneficial Exposome study. The project examines how passive exposure to natural scents, including hinoki and lemon essential oils, may influence daily physiological markers collected through Fitbit wearables.

## Project Overview

Participants completed a longitudinal crossover protocol with a baseline period, intervention periods, water-control periods, and washout periods. Wearable data were processed to evaluate within-participant changes in resting heart rate, heart rate variability, sleep, activity, breathing rate, oxygen saturation, and skin temperature.

Participant-normalized z-scores were calculated relative to each participant’s control period to compare physiological changes across treatment conditions.

## Repository Structure

```
├── data/                 # Input data files, if included 
├── scripts/              # Main analysis scripts 
├── outputs/              # Generated figures, tables, and model outputs 
├── README.md             # Project documentation 
└── requirements.txt      # Package requirements, if applicable 
```

## Getting Started

To access and run the code, clone this repository:

```
bash git clone https://github.com/tyyang05/beneficial_exposome.git
cd YOUR-REPOSITORY 
```

If using R, open the project folder in RStudio and run the analysis scripts from the repository root directory.

## Running the Analysis

Analysis scripts can be run from the scripts/ folder. For example:

r source("scripts/your_analysis_script.R") 

The workflow generally includes:

1. Loading and cleaning wearable data  
2. Aligning data by participant, study period, and treatment condition  
3. Calculating participant-normalized baseline z-scores  
4. Fitting linear mixed-effects models  
5. Generating summary tables and figures  

## Statistical Approach

Wearable outcomes were normalized within each participant using baseline means and standard deviations. Linear mixed-effects models were used to evaluate treatment-associated changes while accounting for repeated measures within participants.

## Notes on Data Access

Raw participant-level wearable data are not included in this repository because they may contain sensitive or identifiable health information. Code is provided for reproducibility and can be adapted to similarly structured datasets.

## Contact

For questions about this repository, please contact:

Tyler Yang  
tyyang@stanford.edu

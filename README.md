# Acetylcholinesterase-Data-Analysis

Exploratory Data Analysis on Acetylcholinesterase Inhibitors
Overview

This project focuses on performing Exploratory Data Analysis (EDA) and molecular descriptor-based analysis on compounds that target the enzyme Acetylcholinesterase (AChE) — a key enzyme involved in neurotransmission and a major target in Alzheimer’s disease research.
The goal is to analyze molecular features, evaluate drug-likeness, and identify patterns among compounds with potential inhibitory activity against AChE.

Objectives

Analyze and visualize data related to AChE inhibitors.

Generate and interpret molecular descriptors and fingerprints to characterize compounds.

Assess drug-likeness using Lipinski’s Rule of Five.

Explore relationships between molecular properties and bioactivity using statistical and visual methods.

Gain insight into the structure–activity relationship (SAR) of AChE-targeting compounds.

Tools & Libraries Used

Python (Data analysis and computation)

RDKit – For molecular structure handling, descriptor generation, and fingerprint creation

PaDEL-Descriptor – For large-scale descriptor and fingerprint computation

ChEMBL Database – As a bioactivity data source for AChE inhibitors

Pandas / NumPy – Data cleaning, aggregation, and manipulation

Matplotlib / Seaborn – Visualization and trend analysis

scikit-learn – For data preprocessing and optional exploratory ML modeling

Project Workflow

Data Collection

Retrieved AChE bioactivity data from the ChEMBL database.

Cleaned and formatted data for descriptor analysis.

Descriptor Generation

Calculated molecular descriptors and fingerprints using RDKit and PaDEL-Descriptor.

Each compound was represented numerically for statistical and comparative analysis.

Data Processing & Analysis

Removed missing or redundant data.

Classified compounds into active, intermediate, and inactive groups based on IC50 values.

Explored distributions, correlations, and feature patterns across compound classes.

Drug-Likeness Evaluation

Applied Lipinski’s Rule of Five to identify potentially drug-like compounds.

Compared property distributions (e.g., molecular weight, LogP, H-bond donors/acceptors).

Visualization & Insights

Created histograms, scatterplots, and correlation heatmaps to identify property trends.

Highlighted key features correlated with AChE inhibitory activity.

Results & Insights

Found consistent property patterns distinguishing active inhibitors from inactives.

Identified correlations between molecular weight, LogP, and bioactivity.

Lipinski analysis revealed a subset of compounds that meet typical drug-likeness criteria.

Descriptor analysis showed potential for future QSAR modeling or predictive screening.

Repository Structure
Acetylcholinesterase-EDA/
│
├── data/
│   ├── bioactivity_data.csv
│   ├── descriptors_output.csv
│   └── cleaned_data.csv
│
├── notebooks/
│   ├── 01_data_preparation.ipynb
│   ├── 02_descriptor_generation.ipynb
│   ├── 03_analysis_visualization.ipynb
│
├── results/
│   ├── figures/
│   │   ├── correlation_heatmap.png
│   │   └── activity_distribution.png
│   └── summary_report.csv
│
├── requirements.txt
├── README.md
└── LICENSE

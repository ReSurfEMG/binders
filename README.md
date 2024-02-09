<h1 align="center">
    <img style="width: 35%; height: 35%" src="https://github.com/resurfemg/resurfemg/blob/main/Logo_rond_tekst.svg"> Binders
</h1>

# Introduction
This repository provides binders accompanying the publications published using the ReSurfEMG software library. ReSurfEMG is an open source collaborative Python library for analysis of respiratory electromyography (EMG). On the same site as the repository for this library we keep related resources.

# Binders
Binders are integrated packages of code that run online in a webbrowser. In that way, you can use the code without installing anything. The binders in this repository are Jupyter Notebook binders, which allow for a step-wise code execution. In between the code snippets (so called "cells"), the outputs are shown in the form of text, tables, and figures.

The binder consist of several notebooks. To go to the main landing page of the binder, click this button:  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ReSurfEMG/binders/main)

## *Advanced waveform analysis of diaphragm surface EMG allows for continuous non-invasive assessment of respiratory effort in critically ill patients at different PEEP levels*
Two notebooks accompany this publication. Click the associated buttons to directly go to these binders:
- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ReSurfEMG/binders/main?labpath=neuromuscular_coupling_quality_assessment_for_pub_synthetic_data.ipynb) - Synthetic data  
    This binder generates synthetic data online and allows for quick evaluation of the data analysis methodology in the paper.
- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ReSurfEMG/binders/main?labpath=neuromuscular_coupling_quality_assessment_for_pub.ipynb) - Load data  
    This binder imports data from the 'synthetic_data' folder, and runs as it would with 'real' patient data. 
-   Run with your own data  
    When downloaded and run in an environment as specified in the environment.yml file, the script can be run with your own data. To do so, take the following steps:
    - Install a [Conda](https://docs.conda.io/projects/miniconda/en/latest/) version compatible with your system.
    - Run the Conda command prompt
    - Create a Conda environment
        ```conda
        conda env create -f environment.yml
        ```
    - Activate the environment
        ```conda
        conda activate resurfemg_binder
        ```
    - Start the Jupyter server
        ```conda
        jupyter notebook
        ```
        The web-based Jupyter notebook automatically opens, or click the appearing link.
    -   Set the file path to be the following directory
        ```python
        root_patient_data_directory = '{OWN_FILE_PATH}'
        ```
    

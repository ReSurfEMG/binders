<h1 align="center">
    <img style="width: 35%; height: 35%" src="https://github.com/resurfemg/resurfemg/blob/main/Logo_rond_tekst.svg"> Binders
</h1>

# Introduction
This repository provides binders accomponying the publications published using the ReSurfEMG software library. ReSurfEMG is an open source collaborative Python library for analysis of respiratory electromyography (EMG). On the same site as the repository for this library we keep related resources.

# Binders
Binders are integrated packages of code that run online in a webbrowser. In that way, you can use the code without installing anything. The binders in this repository are Jupyter Notebook binders, which allow for a step-wise code execution. In between the code snippets (so called "cells"), the outputs are shown in the form of text, tables, and figures.

The binder consist of several notebooks. To go to the main landing page of the binder, click this button:  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ReSurfEMG/binders/main)

## *Advanced waveform analysis of the diaphragm surface EMG for continuous non-invasive assessment of the respiratory effort in critically ill patients at different PEEP levels*
Two notebooks accompany this publication. Click the associated buttons to directly go to these binders:
- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ReSurfEMG/binders/e773c90655927f6c7b06df8e97ebc76dbde290c8?urlpath=lab%2Ftree%2Fneuromuscular_coupling_quality_assessment_for_pub_synthetic_data.ipynb) - Synthethic data  
    This binder generates synthetic data inline and allows for quick evaluation of the data analysis methodology in the paper.
- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ReSurfEMG/binders/e773c90655927f6c7b06df8e97ebc76dbde290c8?urlpath=lab%2Ftree%2Fneuromuscular_coupling_quality_assessment_for_pub.ipynb) - Load data  
    This binder imports data from 'synthetic_data' folder. 
-   Run with your own data  
    When downloaded and run in an environment as specified in the environment.yml file, the script can be run with your own data.  To to so, take the following steps:
    - Install a [Conda](https://docs.conda.io/projects/miniconda/en/latest/) version compatatible with your system.
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
    

# Characterisation of genetically encoded hydrogen peroxide sensor dynamics

This repository contains the Supporting Information for the paper 
*"Characterisation of genetically encoded hydrogen peroxide sensor dynamics"* 
by Lind, Rohwer, Veal and Pillay. 

## Computational environment

To set up your own computational environment in order to run the code in this repository,
perform the following steps:

1. Clone this repository:
    ```shell
    git clone https://github.com/redoxsysbio/Redox-sensor-quantification.git 
    ```

2. Create a new Python environment, either using Anaconda 
  (`conda env create -n redox_sensors`) or the Python venv module
   (`python -m venv redox_sensors`). Activate the environment.

3. Install the required Python packages:
    ```shell
    pip install -r requirements.txt
    ```

4. Start jupyter-lab:
    ```shell
    jupyter-lab 
    ```

## Repository contents

The repository is organised into folders:

- **Analysis_code_for_scripting**<br>
  Contains a Python script to calculate signal parameters from input data (time, signal intensity).
  This can be run as a stand-alone script, or the code can be pasted into a Jupyter notebook.
  An example notebook using Google Colab is presented here:
  https://colab.research.google.com/drive/1PzkLiZoITGU8Qo89Foz1TjSLOKaUvMdW?usp=sharing

- **Code_for_main_paper**<br>
  Contains a Jupyter notebook and data in Excel files to recreate all the results from the main paper.
  Open the notebook in Jupyter-Lab and execute the cells one-by-one by selecting the
  cell and pressing `Shift-Enter`.

- **Excel**<br>
  An Excel spreadsheet to calculate the signalling parameters.

## Live notebook instance

Note that a live notebook instance to calculate signal parameters, using the
[JupyterLite](https://jupyterlite.readthedocs.io/) framework, is provided here:
https://redoxsysbio.github.io/signalparameters

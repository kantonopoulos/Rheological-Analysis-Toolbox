# Rheological Analysis Toolbox
***
## Table of Contents
1. [Introduction](#introduction)
2. [What can I do with the Rheological Analysis Toolbox?](#what-can-i-do-with-the-rheological-analysis-toolbox?)
3. [License](#license)
4. [Installation](#installation)

## Introduction
The Rheological Analysis Toolbox is a comprehensive set of tools designed for performing rheological analysis and data processing of synovial fluid samples. Its main purpose is to aid in the diagnosis of Osteoarthritis (OA) by analyzing the rheological properties of synovial fluid samples. This toolbox has been developed as part of a research project aimed at creating a medical device for OA diagnosis based on rheological data.

**Python Version: 3.11.3**

## What can I do with the Rheological Analysis Toolbox?
The Rheological Analysis Toolbox offers a wide range of functionalities, empowering researchers and medical practitioners to perform comprehensive analysis of synovial fluid samples and derive valuable insights. The key capabilities of the toolbox include:

* Database Creation: Facilitates the creation of a dedicated database to store samples' profile information, ensuring efficient organization and management of the data.
* Sample Analysis: Analyze synovial fluid samples using various rheological tests, including time sweep, frequency sweep, flow step, and the Cox-Merz rule. These analyses help to understand the viscoelastic properties of the samples.
* Database Augmentation: Automatically appends the results of rheological analyses to the primary database, allowing for further in-depth analysis and comparison.
* Technical Report Generation: Automates the process of generating technical reports for each sample, providing comprehensive and detailed documentation.
* Data Preprocessing: Offers data preprocessing functionalities, enabling researchers to clean and prepare the data for further analysis.
* Data Categorization: Categorizes samples into subsets based on specific characteristics, facilitating targeted analysis and comparisons.
* Statistical Analysis: Provides statistical analysis tools to gain insights into general data statistics and perform an independent two-sample t-test for comparative studies.
* Biomarker Validation: Enables researchers to validate biomarkers, aiding in the identification of potential biomarkers associated with OA.
* Data Visualization: Allows researchers to create custom, ready-to-publish box plots for visually representing and interpreting the data.

## License
The Rheological Analysis Toolbox is licensed under the "Laboratory Use License" agreement. This license is exclusively intended for use within the Biomedical Lab of the Chemical Engineering Faculty at Aristotle University of Thessaloniki. The use of the toolbox is limited to researchers, staff, and students affiliated with the lab for academic and research purposes.

## Installation
### Recommended Step: Anaconda Installation
1. Download and install the Anaconda distribution from the official website: [Anaconda](https://www.anaconda.com/). Follow the installation instructions provided by Anaconda to install the distribution on your computer, including access to Jupyter Notebook and Jupyter Lab.

### Required Steps: Package Installation
If you have installed Anaconda:
Open the Anaconda Navigator or Anaconda Prompt and install the required packages using the following commands:
```
conda install -c conda-forge fpdf
conda install -c conda-forge prettytable
```
If you have not installed Anaconda:
1. Download and install Python 3.8 or later from the official Python website: [Python](https://www.python.org/downloads/).
2. Open the command prompt (Windows) or terminal (macOS, Linux).
3. Install the required packages using pip:
```
pip install openpyxl
pip install numpy
pip install pandas
pip install seaborn
pip install matplotlib
pip install plotly
pip install ipywidgets
pip install prettytable
pip install fpdf
pip install scipy
```

### Getting the Code
Clone the Rheological Analysis Toolbox repository from GitHub using the following command:
```
git clone https://github.com/Synovial-Fluid-Research-Programme/Rheological-Analysis-Toolbox.git
```
Alternatively, you can download the repository as a ZIP file from the GitHub page and extract it to a local directory.

### Running the Code
1. Navigate to the directory where you cloned or extracted the repository.
2. Launch Jupyter Notebook, Jupyter Lab, or any Python IDE.
3. Open the relevant notebook files (*.ipynb) in Jupyter (or Python Files if using other IDE) and execute the code cells to run the Rheological Analysis Toolbox.

Now you are ready to perform rheological and data analysis of synovial fluid samples and further develop the OA diagnostic medical device. For more detailed documentation and instructions, please refer to the complete documentation provided.
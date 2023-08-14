# Rheological Analysis Toolbox
***
## Table of Contents
1. [Introduction](#introduction)
2. [What can I do with the Rheological Analysis Toolbox?](#what-can-i-do-with-the-rheological-analysis-toolbox?)
3. [License](#license)
4. [Installation](#installation)
5. [Contributing](#contributing)

## Introduction
The Rheological Analysis Toolbox is a comprehensive set of tools designed for performing rheological analysis and data processing of synovial fluid samples. Its main purpose is to aid in the diagnosis of Osteoarthritis (OA) by analyzing the rheological properties of synovial fluid samples. This toolbox has been developed as part of a research project aimed at creating a medical device for OA diagnosis based on rheological data.

**Python Version: 3.8 or later**

The full documentation and examples can be found in this [link](https://north-mandevilla-d3a.notion.site/Rheological-Analysis-Toolbox-caf04f0f4f2c4d30b31cbca9400580f0?pvs=4).

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
* Data Sampling: Researchers can sample their data and produce DataFrames with great numbers of artificial samples simulating the real data distributions.
* Training and Evaluation of Machine Learning Models: The toolbox can train and validate machine learning models, such as Logistic Regression models and evaluate them with multiple techniques, such as cross-validation or ROC analysis.

## License
The Rheological Analysis Toolbox is licensed under the "Laboratory Use License" agreement. This license is exclusively intended for use within the Biomedical Lab of the Chemical Engineering Faculty at Aristotle University of Thessaloniki. The use of the toolbox is limited to researchers, staff, and students affiliated with the lab for academic and research purposes. The full license can be found in this [link](https://github.com/Synovial-Fluid-Research-Programme/Rheological-Analysis-Toolbox/blob/main/LICENSE).

## Installation
### Recommended Step: Anaconda Installation
1. Download and install the Anaconda distribution from the official website: [Anaconda](https://www.anaconda.com/). Anaconda provides pre-installed packages and Jupyter Notebook access by default. Follow the installation instructions provided by Anaconda to install the distribution on your computer, including access to Jupyter Notebook and Jupyter Lab.

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
pip install -U openpyxl
pip install -U numpy
pip install -U pandas
pip install -U seaborn
pip install -U matplotlib
pip install -U plotly
pip install -U ipywidgets
pip install -U prettytable
pip install -U fpdf
pip install -U scipy
pip install -U scikit-learn
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

## Contributing
Researchers from the Biomedical Lab of the Chemical Engineering Department at Aristotle University of Thessaloniki are encouraged to actively contribute to the development and enhancement of the Rheological Analysis Toolbox. Contributions may include bug fixes, new features, code optimizations, documentation improvements, and more.

### How to Contribute
1. Fork the repository on GitHub to create a copy of the project in your GitHub account.
2. Clone the forked repository to your local development environment.
3. Create a new branch for your contributions. Use a descriptive name that reflects the nature of your changes.
4. Implement your changes, additions, or improvements in the codebase.
5. Commit your changes and provide clear and concise commit messages.
6. Push your changes to your GitHub repository.
7. Submit a pull request to the original repository, describing the changes you have made and the purpose of your contribution.
Your pull request will be reviewed by the maintainers, and feedback or additional changes may be requested. Once your contribution is approved, it will be merged into the main repository, and your work will be acknowledged in the project's history.

### Contact Information
For any inquiries, questions, or discussions related to the Rheological Analysis Toolbox or its development, please feel free to reach out to:

Name: Konstantinos Antonopoulos | Email: k.antono@outlook.com

We welcome your active participation and collaboration in making the Rheological Analysis Toolbox a valuable resource for rheological analysis and data processing in the field of Osteoarthritis diagnosis. Together, we can advance research and contribute to the improvement of medical knowledge in this important area. Thank you for your contributions!

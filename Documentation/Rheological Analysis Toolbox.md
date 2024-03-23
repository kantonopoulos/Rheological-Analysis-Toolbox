# Rheological Analysis Toolbox

Created By: Kostas Antonopoulos
Created: July 27, 2023 10:07 PM
Last Edited Time: August 8, 2023 3:47 PM
Last Edited By: Kostas Antonopoulos

> 📘 Any questions or thoughts? You can contact me at **k.antono@outlook.com**.
> 

# Contents

# Chapter 1 - Introduction

## What is the Rheological Analysis Toolbox?

The Rheological Analysis Toolbox is a comprehensive and powerful set of tools designed to perform rheological analysis and data processing of synovial fluid samples. The primary objective of this toolbox is to facilitate the diagnosis of Osteoarthritis (OA) by analyzing the rheological properties of the synovial fluid samples. The toolbox has been developed as part of a research project aimed at creating a medical device for OA diagnosis based on rheological data.

Rheology is the study of the flow and deformation of materials under applied forces. In the context of synovial fluid analysis, rheology plays a crucial role in understanding the mechanical behavior of this biological fluid, which is directly associated with joint health and OA. By analyzing the rheological properties of synovial fluid samples, researchers and medical professionals can gain valuable insights into the presence and severity of OA.

The Rheological Analysis Toolbox serves as a knowledge management and transfer resource for researchers working in the Biomedical Lab of the Chemical Engineering Faculty at Aristotle University of Thessaloniki. It provides a standardised and efficient way to process, analyze, and interpret rheological data from synovial fluid samples, enabling researchers to make informed decisions and draw meaningful conclusions.

**Python Version: 3.8 or later**.

## What can I do with the Rheological Analysis Toolbox?

The Rheological Analysis Toolbox offers a wide range of functionalities, empowering researchers and medical practitioners to perform comprehensive analysis of synovial fluid samples and derive valuable insights. The key capabilities of the toolbox include:

1. **Database Creation**: The toolbox facilitates the creation of a dedicated database to store samples' profile information, ensuring efficient organization and management of the data.
2. **Sample Analysis**: Researchers can analyze synovial fluid samples using various rheological tests, including the tests time sweep, frequency sweep, flow step, and the Cox-Merz rule. These analyses help to understand the viscoelastic properties of the samples.
3. **Database Augmentation**: The results of the rheological analyses are automatically appended to the primary database, allowing for further in-depth analysis and comparison.
4. **Technical Report Generation**: The toolbox automates the process of generating technical reports for each sample, providing researchers with comprehensive and detailed documentation.
5. **Data Preprocessing**: The toolbox offers data preprocessing functionalities, enabling researchers to clean and prepare the data for further analysis.
6. **Data Categorization**: Researchers can categorize samples into subsets based on specific characteristics, facilitating targeted analysis and comparisons.
7. **Statistical Analysis**: The toolbox provides statistical analysis tools to gain insights into general data statistics and perform an independent two-sample t-test for comparative studies.
8. **Biomarker Validation**: Researchers can validate biomarkers using the toolbox, aiding in the identification of potential biomarkers associated with OA.
9. **Data Visualization**: The toolbox enables researchers to create custom, ready-to-publish box plots for visually representing and interpreting the data.
10. **Data Sampling**: Researchers can sample their data and produce DataFrames with great numbers of artificial samples simulating the real data distributions.
11. **Training and Evaluation of Machine Learning Models**: The toolbox can train and validate machine learning models, such as Logistic Regression models and evaluate them with multiple techniques, such as cross-validation or ROC analysis.

The Rheological Analysis Toolbox streamlines the entire process of synovial fluid analysis, from data collection to visualization and interpretation. It empowers researchers to make data-driven decisions, enhances research efficiency, and contributes to the advancement of medical knowledge in the field of Osteoarthritis diagnosis.

<aside>
💡 Before utilizing the toolbox, ensure that you have a basic understanding of rheology, data analysis, and the specific protocols for synovial fluid sample analysis. Additionally, the toolbox requires the installation of relevant Python libraries, such as NumPy, Pandas, SciPy, and Seaborn, to function effectively.

</aside>

## License

The Rheological Analysis Toolbox is licensed under the "Laboratory Use License" agreement. This license is exclusively intended for use within the Biomedical Lab of the Chemical Engineering Faculty at Aristotle University of Thessaloniki. The use of the toolbox is limited to researchers, staff, and students affiliated with the lab for academic and research purposes.

### **Terms and Conditions**

1. **Restricted Use**: The Rheological Analysis Toolbox can only be used within the premises of the Biomedical Lab at Aristotle University of Thessaloniki. It is strictly prohibited to share, distribute, or transfer the toolbox to any external party without prior written consent.
2. **Confidentiality**: The toolbox and its source code contain confidential and proprietary information. Users are required to maintain the utmost confidentiality and protect the toolbox from any unauthorized access or disclosure.
3. **Commercialization Limitation**: The use of the Rheological Analysis Toolbox is restricted to academic research purposes and the development of the OA diagnostic medical device within the lab. Commercialization of any aspect of the toolbox or its outputs is strictly prohibited without written authorization from the lab's management.
4. **Non-Commercial Distribution**: Researchers and users within the lab are permitted to collaborate and share the outputs of the toolbox for non-commercial research purposes within the lab. However, any distribution of the toolbox or its outputs to external parties must be compliant with the terms and conditions of this license.
5. **Attribution**: All users are required to acknowledge and credit the Biomedical Lab of the Chemical Engineering Faculty at Aristotle University of Thessaloniki as the developer and owner of the Rheological Analysis Toolbox in any publications or presentations arising from the use of the toolbox.
6. **Disclaimer of Warranty**: The Rheological Analysis Toolbox is provided "as is" without any warranties or guarantees of any kind, expressed or implied. The lab's management shall not be liable for any damages or losses arising from the use or inability to use the toolbox.
7. **Termination**: The Biomedical Lab reserves the right to terminate this license and revoke access to the Rheological Analysis Toolbox at any time and for any reason.

By using the Rheological Analysis Toolbox, users agree to be bound by the terms and conditions of this license. Any violation of these terms may result in disciplinary action and legal consequences.

For inquiries about the license, permission for external use, or any other related matters, please contact the lab's management or the designated person responsible for the toolbox administration.

---

# Chapter 2 - Installation

## **Recommended Step: Anaconda Installation**

1. Visit the official Anaconda website at **[https://www.anaconda.com/](https://www.anaconda.com/)** and download the latest Anaconda distribution suitable for your operating system (Windows, macOS, or Linux).
2. Follow the installation instructions provided by Anaconda to install the distribution on your computer.
3. During the installation, make sure to select the option to install all preinstalled packages and to include access to both Jupyter Notebook and Jupyter Lab.

## **Required Steps: Package Installation**

### If you have installed Anaconda:

1. Open the Anaconda Navigator or Anaconda Prompt.
2. Install the required packages using the following commands:
    
    ```powershell
    # Install the required packages using conda
    conda install -c conda-forge fpdf
    conda install -c conda-forge prettytable
    ```
    

### If you have not installed Anaconda:

1. Download and install Python 3.8 or later from the official Python website: **[https://www.python.org/downloads/](https://www.python.org/downloads/)**
2. Open the command prompt (Windows) or terminal (macOS, Linux).
3. Install the required packages using pip:
    
    ```powershell
    # Install the required packages using pip
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
    

### **Getting the Code**

1. Clone the Rheological Analysis Toolbox repository from GitHub using the following command:
    
    ```powershell
    git clone https://github.com/Synovial-Fluid-Research-Programme/Rheological-Analysis-Toolbox.git
    ```
    
2. Alternatively, you can download the repository as a ZIP file from the GitHub page and extract it to a local directory.

### **Running the Code**

1. Navigate to the directory where you cloned or extracted the repository.
2. Launch Jupyter Notebook, Jupyter Lab, or any IDE.
3. Open the relevant notebook files (*.ipynb) in Jupyter (or Python Files if using other IDE) and execute the code cells to run the Rheological Analysis Toolbox.

The library is now ready to be used for performing rheological and data analysis of synovial fluid samples and further developing the OA diagnostic medical device.

<aside>
‼️ Even though, it is not required, it is strongly recommended to download, install and use the Anaconda Distribution and Jupyter Notebook, while using this toolbox. It will make its installation and the overall user experience simpler and more efficient.

</aside>

# Chapter 3 - Database Creator

## Helper **Function: create_new_workbook(file_name, column_labels)**

### **Description**

This function creates a new workbook in Excel with the given **`file_name`** and adds the provided **`column_labels`** as the header for the columns.

### **Parameters**

- **`file_name`** (str): The name of the Excel file to be created.
- **`column_labels`** (list): A list of strings representing the header labels for the columns.

### **Returns**

- **`None`**: The function does not return any value explicitly; it creates the new workbook and adds the specified **`column_labels`** to it.

### **Behavior**

1. The function creates a new Excel workbook using the openpyxl library.
2. It sets the active worksheet of the workbook.
3. The function then appends the **`column_labels`** list to the worksheet, which sets the header labels for the columns.
4. Finally, it saves the workbook with the given **`file_name`**.

## Helper **Function: get_unique_file_name(file_name)**

### **Description**

This function generates a unique file name by appending a number to the original **`file_name`** to avoid naming conflicts with existing files.

### **Parameters**

- **`file_name`** (str): The name of the Excel file.

### **Returns**

- **`str`**: A unique file name with a number appended to it.

### **Behavior**

1. The function first splits the **`file_name`** into two parts: the base name and the extension.
2. It initializes a counter to 1.
3. The function generates a unique file name by appending the counter and the original extension to the base name, separated by an underscore.
4. It then checks if the file with the generated unique name already exists in the current directory.
5. If the file exists, it increments the counter and generates a new unique name, repeating the check until it finds an unused name.
6. Once a unique name is found, the function returns it.

## **Function: create_database(file_name, column_labels)**

### **Description**

This function creates a new Excel database file as an empty workbook with specified column headers. If a file with the given **`file_name`** already exists, the function provides the user with options to either replace the existing file or create a new file with a unique name to prevent overwriting.

### **Parameters**

- **`file_name`** (str): The name of the Excel file to be created or modified.
- **`column_labels`** (str): The column labels for the database. This should be a list of strings, where each string represents a header label for the columns.

### **Returns**

- **`None`**: The function does not return any value explicitly; it either creates the new database or updates the existing one.

### **Behavior**

1. The function first checks if a file with the given **`file_name`** already exists in the current directory using the helper function `**get_unique_file_name(file_name)**`.
2. If the file exists, it prompts the user to choose between replacing the file or adding to it.
    - If the user chooses to replace ('R'), the function creates a new Excel workbook with the specified **`file_name`** and the provided **`column_labels`**, overwriting the existing file.
    - If the user chooses to add ('A'), the function appends a number to the **`file_name`** to make it unique, then creates a new Excel workbook with this unique name and the provided **`column_labels`**.
    - If the user inputs an invalid choice, the program displays an error message and exits.
3. If the file does not exist, the function directly creates a new Excel workbook with the provided **`file_name`** and **`column_labels`** using the helper function `**create_new_workbook(file_name, column_labels)**`.

### Calling Example

Via the following example code two databases are created, "Database.xlsx" and "Statistical_Analysis_Database.xlsx" Excel databases respectively. The sample’s profile information are going to be stored in the first, while the second is the primary database that is going to be used from the data analysis pipeline. It consists of the results of the rheological analysis, as well as some data from the first database.

```python
# Create first database
file_name = "Database.xlsx"
column_labels = ['ID', 'Date', 'Gender', 'Age', 'Joint', 'Condition', 'Total Volume (mL)', 'Color', 
                     'Transparency', 'Texture', 'Blood', 'Clot', 'Tissue', 'Storage in freezer', 'COVID 19', 
                     'Vaccinated COVID 19', 'COVID 19 now', 'Number of Tests', 'Test Type', 
                     'Temperature (oC)', 'Tissue in Test', 'Bubbles before Test', 'Bubbles after Test']
create_database(file_name, column_labels)

# Create final database
file_name2 = "Statistical_Analysis_Database.xlsx"    
column_labels2 = ["ID", "Gender", "Age", "Joint", "Condition", "Blood", "Clot", "Tissue", 
                     "Tissue or Clot in Test", "Storage in freezer", "COVID 19", 
                     "Vaccined COVID 19", "COVID 19 now", "Time Sweep G' average (Pa)", 
                     "Time Sweep G'' average (Pa)", "Time Sweep G' standard deviation (-)", 
                     "Time Sweep G'' standard deviation (-)", "Frequency Sweep G' at 0.68 rad/s (Pa)", 
                     "Frequency Sweep G'' at 0.68 rad/s (Pa)", "Frequency Sweep G' at 3.142 rad/s (Pa)", 
                     "Frequency Sweep G'' at 3.142 rad/s (Pa)", "Frequency Sweep G' at 14.58 rad/s (Pa)", 
                     "Frequency Sweep G'' at 14.58 rad/s (Pa)", "Cross Over Point (rad/s)", 
                     "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)", 
                     "Zero-rate Viscosity (Pa.s)", "Infinite-rate Viscosity (Pa.s)", "Consistency (s)", 
                     "Rate Index (-)", "Standard Error (-)", "Flow Step Viscosity at 3.162 1/s (Pa.s)"]
create_database(file_name2, column_labels2)
```

---

# Chapter 4 - New Sample Profile Creator

## Helper **Function: get_valid_integer(prompt)**

### **Description**

This function prompts the user to input a valid integer and repeatedly asks for input until a valid integer is provided.

### **Parameters**

- **`prompt`** (str): The prompt message for the user.

### **Returns**

- **`int`**: A valid integer provided by the user.

### **Behavior**

1. The function enters an infinite loop.
2. It prompts the user with the **`prompt`** message and collects the user input, stripping any leading or trailing whitespaces.
3. If the input is not a valid integer (i.e., it contains non-numeric characters), the function prints an error message and asks for input again.
4. If the input is a valid integer, the function converts the input to an integer and returns it, exiting the loop.

## Helper **Function: get_valid_float(prompt)**

### **Description**

This function prompts the user to input a valid float and repeatedly asks for input until a valid float is provided.

### **Parameters**

- **`prompt`** (str): The prompt message for the user.

### **Returns**

- **`float`**: A valid float provided by the user.

### **Behavior**

1. The function enters an infinite loop.
2. It prompts the user with the **`prompt`** message and collects the user input, stripping any leading or trailing whitespaces.
3. It tries to convert the input to a float using a **`try-except`** block.
4. If the conversion succeeds (i.e., the input is a valid float), the function returns the float value and exits the loop.
5. If the conversion fails due to a **`ValueError`**, the function prints an error message and asks for input again.

## Helper **Function: get_valid_date()**

### **Description**

This function prompts the user to input a valid date in the format "DD/MM/YYYY" and repeatedly asks for input until a valid date is provided.

### **Parameters**

- **`None`.**

### **Returns**

- **`str`**: A valid date in the format "DD/MM/YYYY".

### **Behavior**

1. The function enters an infinite loop.
2. It prompts the user with the message "Date: (DD/MM/YYYY)" and collects the user input, stripping any leading or trailing whitespaces.
3. It tries to parse the input as a date using the **`datetime.datetime.strptime()`** method with the format "%d/%m/%Y".
4. If the parsing succeeds (i.e., the input is a valid date), the function returns the date in string format and exits the loop.
5. If the parsing fails due to a **`ValueError`**, the function prints an error message and asks for input again.

## Helper **Function: get_valid_input(prompt, valid_values=None)**

### **Description**

This function prompts the user to input valid data based on the provided prompt and a list of valid values (if applicable) and repeatedly asks for input until valid data is provided.

### **Parameters**

- **`prompt`** (str): The prompt message for the user.
- **`valid_values`** (list, optional): A list of valid values (strings) if applicable. If provided, the user's input must match one of the valid values from the list.

### **Returns**

- **`str`**: Valid input provided by the user.

### **Behavior**

1. The function enters an infinite loop.
2. It prompts the user with the **`prompt`** message and collects the user input, converting it to lowercase and stripping any leading or trailing whitespaces.
3. If **`valid_values`** is not None, the function checks if the input is in the list of **`valid_values`**. If it is not, the function prints an error message along with the list of valid values and asks for input again.
4. If the input is an empty string, the function prints an error message and asks for input again.
5. If the input is valid (i.e., it matches one of the **`valid_values`** or is not empty), the function returns the input and exits the loop.

## Helper **Function: sdescription()**

### **Description**

This function collects and processes sample data from user input. It prompts the user for various sample attributes and allows the user to revise the input data before saving it.

### **Parameters**

- **`None`**.

### **Returns**

- **`list`**: A list containing sample information in the following order:
**`[Sample ID, Date, Gender, Age, Joint, Condition, Total Volume (mL), Color, Transparency, Texture, Blood, Clot, Tissue, Storage in freezer, COVID-19, Vaccinated for COVID-19, COVID-19 now, Number of Tests]`**

### **Behavior**

1. The function initializes an empty list **`sdesc`** to store the sample data.
2. It prompts the user to input various sample attributes using the helper functions **`get_valid_integer()`**, **`get_valid_float()`**, **`get_valid_date()`**, and **`get_valid_input()`**.
3. After collecting all the sample attributes, it prints the input data for review.

1. The user is then prompted to confirm or revise the input data. If the user chooses to revise, they can choose which data point to update and enter the revised value.
2. The function then returns the list **`sdesc`**, containing all the sample information.

## Helper **Function: tdescription(my_list)**

### **Description**

This function collects and processes test data from user input. It prompts the user for various test attributes based on the sample information provided in the **`my_list`** parameter.

### **Parameters**

- **`my_list`** (list): A list containing sample information in the following order:
**`[Sample ID, Date, Gender, Age, Joint, Condition, Total Volume (mL), Color, Transparency, Texture, Blood, Clot, Tissue, Storage in freezer, COVID-19, Vaccinated for COVID-19, COVID-19 now, Number of Tests]`**

### **Returns**

- **`list`**: A list containing test information for each test in the following order:
**`[Test Type, Temperature (oC), Tissue in Test, Bubbles before Test, Bubbles after Test]`**

### **Behavior**

1. The function initializes an empty list **`tdesc`** to store the test data.
2. It extracts the sample attributes relevant to test data from the provided **`my_list`**.
3. It prompts the user to input various test attributes using the helper functions **`get_valid_input()`** based on the sample information.
4. After collecting all the test attributes for one test, it prints the input data for review.
5. The user is then prompted to confirm or revise the input data. If the user chooses to revise, they can choose which data point to update and enter the revised value.
6. The process of collecting test data is repeated for the number of tests provided in the sample information.
7. The function returns the list **`tdesc`**, containing all the test information for each test.

## **Function: append_sample_to_database(file_name="Database.xlsx")**

### **Description**

This function appends new sample and its profile data to an existing Excel database. It collects the sample information using the **`sdescription()`** function and test information using the **`tdescription()`** function.

### **Parameters**

- **`file_name`** (str, optional): Name of the Excel file to be updated. Default is "Database.xlsx".

### **Returns**

- **`None`**: The function does not return any value explicitly; it appends the **`sdesc`** and **`tdesc`** lists into an Excel Workbook.

### **Behavior**

1. The function calls the **`sdescription()`** function to collect and process the sample data. It also calls the **`tdescription()`** function to collect and process the corresponding test data for the sample.
2. The function then loads the existing Excel file specified by **`file_name`** using the **`openpyxl.load_workbook()`** method and sets the active worksheet.
3. It finds the next empty row in the Excel sheet to append the new sample data.
4. It appends the sample data to the next empty row in the Excel sheet.
5. For each test associated with the sample, it appends the test data to consecutive rows following the sample data.
6. It fills the remaining columns (A to S) for each row of test data with copies of the corresponding sample data to maintain consistency.
7. Finally, the function saves the changes back to the Excel file using the **`wb.save()`** method.
8. The function prints a message indicating that the data has been saved in the Excel workbook.

### Calling Example

Via the following example command the function collects the sample information and appends them to "Database.xlsx" Excel database.

`**append_sample_to_database(file_name="Database.xlsx")**`

---

# Chapter 5 - Rheology Analyser

## Helper Function: plot_time_sweep_data(df_ts)

### Description

This function plots the time sweep data as a scatter plot, allowing interactive control over the y-axis limits. The interactive plot provides flexibility in adjusting the visualization for better insights.

### Parameters

- **`df_ts`** (DataFrame): The input DataFrame containing the time sweep data.

### **Returns**

- **`None`**: The function does not return any value explicitly; it creates a plot.

### Behavior

- The function generates an interactive scatter plot using the **`interact`** function, where users can adjust the y-axis limits with sliders.
- The plot shows two data series, 'G'' and 'G''', representing G' and G'' values with respect to time (minutes).
- The plot uses a log scale on the y-axis to better visualize the data's magnitude.
- The data is color-coded for easy distinction.
- A legend is displayed to identify the data series.

## Helper Function: time_sweep_data_analysis(df)

### Description

This function performs analysis on the data of time sweep test. It calculates the mean and standard deviation of G' and G'' values within a specified time interval and displays the results in a tabular format.

### Parameters

- **`df`** (DataFrame): The input DataFrame containing the time sweep data.

### Returns

- **`mean_values`** (numpy.array): Array of mean G' and G'' (Pa) values at 3.142 rad/s from the time sweep test.
- **`std_values`** (numpy.array): Array of G' and G'' (Pa) standard deviations from the time sweep test.

### Behavior

- The function first selects the relevant columns from the input DataFrame (**`df`**) related to the time sweep data.
- It plots the data using the helper function **`plot_time_sweep_data()`**.
- It then prompts the user to input start and finish time points for the analysis time interval.
- The function calculates the mean and standard deviation of G' and G'' values within the specified time interval.
- The results are displayed in a tabular format using the **`PrettyTable`** library.
- Finally, the function returns the mean and standard deviation values as a DataFrame.

## Helper Function: plot_frequency_sweep_data(df_fs, frequency_interval)

### Description

This function plots the frequency sweep data as a scatter plot, including a secondary y-axis for the |n*| (Pa.s) values. The interactive plot allows users to adjust the primary y-axis limits.

### Parameters

- **`df_fs`** (DataFrame): The input DataFrame containing the frequency sweep data.
- **`frequency_interval`** (DataFrame): A subset of the **`df_fs`** DataFrame, representing the data within a selected time interval.

### **Returns**

- **`None`**: The function does not return any value explicitly; it creates a plot.

### Behavior

- The function generates an interactive scatter plot using the **`interact`** function, where users can adjust the primary y-axis limits with sliders.
- The plot displays three data series: G', G'', and |n*|, representing G' and G'' values and complex viscosity |n*| with respect to angular frequency (rad/s).
- The plot uses a log scale on both the x-axis and the primary y-axis to better visualize the data's magnitude.
- |n*| is plotted on a secondary y-axis to compare its values with G' and G''.
- The data is color-coded for easy distinction.
- A legend is displayed to identify the data series.

## Helper Function: frequency_sweep_data_analysis(df)

### Description

This function performs analysis on the data of frequency sweep test. It calculates various values such as G', G'', complex viscosity (|n*|), and crossover point. The function prints the crossover point if found, or a message indicating its absence.

### Parameters

- **`df`** (DataFrame): The input DataFrame containing the frequency sweep data.

### Returns

- **`G_pf`** (float): G' (Pa) at 3.142 rad/s from the frequency sweep test.
- **`G_dpf`** (float): G'' (Pa) at 3.142 rad/s from the frequency sweep test.
- **`G_pf1`** (float): G' (Pa) at 0.68 rad/s from the frequency sweep test.
- **`G_dpf1`** (float): G'' (Pa) at 0.68 rad/s from the frequency sweep test.
- **`G_pf2`** (float): G' (Pa) at 14.58 rad/s from the frequency sweep test.
- **`G_dpf2`** (float): G'' (Pa) at 14.58 rad/s from the frequency sweep test.
- **`eta_star`** (float): Complex viscosity (Pa.s) at 3.142 rad/s from the frequency sweep test.
- **`crossover_point`** (float): The cross-over point from the frequency sweep test. If not found, the function prints a message indicating its absence.

### Behavior

- The function first selects the relevant columns from the input DataFrame (**`df`**) related to the frequency sweep data.
- It plots the data using the helper function **`plot_frequency_sweep_data()`**.
- It calculates various values such as G', G'', and complex viscosity (|n*|) at specific angular frequencies.
- The function then identifies the crossover point, where G' and G'' intersect, and prints its value if found.
- The calculated values are returned as individual floats.

## Helper Function: calculate_cross_model_equation(s, eta_0, eta_inf, K, n)

### Description

This function calculates the viscosities using the Cross model equation given the parameters.

### Parameters

- **`s`** (numpy.array): The array of shear rates.
- **`eta_0`** (float): The zero-rate viscosity (Pa.s).
- **`eta_inf`** (float): The infinite-rate viscosity (Pa.s).
- **`K`** (float): The consistency (s).
- **`n`** (float): The rate index (-).

### Returns

- **`numpy.array`**: The calculated viscosities using the Cross model equation.

### Behavior

- The function calculates the viscosities based on the Cross model equation: (eta_0 - eta_inf) / (1 + (s * K) ** n) + eta_inf.
- It returns an array of calculated viscosities using the provided parameters.

## Helper Function: plot_flow_step_data(df_step, s_cross, n_cross, ymin_primary)

### Description

This function plots the flow step data as a scatter plot, including the cross model viscosity and flow step viscosity. Users can adjust the primary y-axis limits to customize the plot.

### Parameters

- **`df_step`** (DataFrame): The input DataFrame containing the flow step data.
- **`s_cross`** (numpy.array): The array of shear rates for the Cross model calculation.
- **`n_cross`** (numpy.array): The calculated viscosities using the Cross model equation.
- **`ymin_primary`** (tuple): The range for the primary y-axis.

### **Returns**

- **`None`**: The function does not return any value explicitly; it creates a plot.

### Behavior

- The function generates a scatter plot showing two data series: flow step viscosity and Cross model viscosity.
- The plot includes the calculated viscosities based on the Cross model using shear rates (**`s_cross`**) and the Cross model equation.
- The flow step viscosity data is color-coded for easy distinction.
- The plot uses a log scale on both the x-axis and the primary y-axis to better visualize the data's magnitude.
- Users can interactively adjust the primary y-axis limits with sliders to customize the plot.
- The data points for both flow step viscosity and Cross model viscosity are plotted with different colors for easy identification.
- The legend displays labels for the two data series: "Flow step viscosity" and "Cross model viscosity."

## Helper Function: flow_step_data_analysis(df)

### Description

This function performs analysis on the flow step data for an Osteoarthritis medical device. It calculates the parameters of the Cross model and the flow step viscosity. Additionally, it returns the standard error of the model to assess its accuracy.

### Parameter

- **`df`** (DataFrame): The input DataFrame containing the flow step data.

### Returns

- **`eta_0`** (float): Zero rate viscosity (Pa.s) from the Cross model.
- **`eta_inf`** (float): Infinite rate viscosity (Pa.s) from the Cross model.
- **`K`** (float): Consistency (Pa.s) from the Cross model.
- **`n`** (float): Exponent (-) from the Cross model.
- **`error`** (float): Deviation of the model (-) from the Cross model.
- **`eta`** (float): Viscosity (Pa.s) at 3.162 1/s from the flow step measurement.

### Behavior

- The function first selects the relevant columns from the input DataFrame (**`df`**) related to the flow step data.
- It extracts the required parameters (**`eta_0`**, **`eta_inf`**, **`K`**, and **`n`**) from the DataFrame.
- It plots the data using the helper function **`plot_flow_step_data()`**.
- Additionally, it retrieves the flow step viscosity (**`eta`**) at a specific shear rate (3.162 1/s).
- The function calculates the deviations of the Cross model from the flow step data and stores it in **`error`**.
- Finally, the function returns all the calculated values as individual floats.

## Helper Function: plot_cox_merz_data(df_cox, ymin_primary)

### Description

This function plots the Cox-Merz data as a scatter plot, including both shear rate and angular frequency. Users can interactively adjust the primary y-axis limits to customize the plot.

### Parameters

- **`df_cox`** (DataFrame): The input DataFrame containing the Cox-Merz data.
- **`ymin_primary`** (tuple): The range for the primary y-axis.

### **Returns**

- **`None`**: The function does not return any value explicitly; it creates a plot.

### Behavior

- The function generates a scatter plot showing two data series: viscosity measured at shear rates and complex viscosity (**`|n*|`**) measured at angular frequencies.
- The plot includes the viscosity data at different shear rates and complex viscosity data at various angular frequencies.
- Users can interactively adjust the primary y-axis limits with sliders to customize the plot.
- The data points for both shear rate and complex viscosity are plotted with different colors for easy identification.
- The legend displays labels for the two data series: "Viscosity" and "|n*|".

## Helper Function: **cox_merz_rule(df)**

### Description

This function performs Cox-Merz analysis for an Osteoarthritis medical device. It calculates the viscosity (eta) at 3.162 1/s from flow step test data and the complex viscosity (eta_star) at 3.142 rad/s from frequency test data. It also generates an interactive plot to visualize the Cox-Merz data.

### Parameters

- **`df`** (DataFrame): The input DataFrame containing the Cox-Merz data. The DataFrame should have the following columns: 'shear rate (1/s)', 'viscosity (Pa.s)', 'ang. Frequency (rad/s)', and '|n*| (Pa.s)'.

### Returns

- **`eta`** (float): Viscosity (Pa.s) at 3.162 1/s from flow step test.
- **`eta_star`** (float): Complex viscosity (Pa.s) at 3.142 rad/s from frequency test.

### Behavior

1. The function selects the specific columns required for the Cox-Merz analysis: 'shear rate (1/s)', 'viscosity (Pa.s)', 'ang. Frequency (rad/s)', and '|n*| (Pa.s)'.
2. It removes any rows containing NaN values from the DataFrame.
3. The function generates an interactive plot using the **`plot_cox_merz_data()`** function to visualize the Cox-Merz data. The y-axis limits of the plot can be adjusted using the **`ymin_primary`** parameter of the interactive plot.
4. The viscosity (eta) and complex viscosity (eta_star) at specific shear rate and angular frequency are extracted from the DataFrame.
5. The function creates a PrettyTable with three columns: 'Experiment', 'Variable', and 'Value', and adds the mean and standard deviation values to the table for 'Flow step' and 'Frequency sweep' experiments.
6. The PrettyTable is printed to the console.
7. The calculated values of eta and eta_star are returned as a dictionary with the keys 'eta' and 'eta_star', respectively.

## Function: **sample_analysis(sid, df_ed="Experimental_Data.xlsx")**

### Description

This function performs sample analysis and prints a results summary for a given sample ID number (snum) using experimental data stored in a DataFrame. The analysis results are returned as a dictionary.

### Parameters

- **`sid`** (str): The sample ID to be analyzed.
- **`df_ed`** (DataFrame, optional): The input DataFrame containing the experimental data. The default value is "Experimental_Data.xlsx", assuming that the data is loaded from an Excel file.

### Returns

- **`dict`**: A dictionary containing the analysis results. The dictionary has the following keys:
    - **`'time_sweep'`**: Contains the mean_values and std_values of the time sweep data if present in the DataFrame.
    - `**'frequency_sweep'**`: Contains various rheological parameters (G_pf, G_dpf, G_pf1, G_dpf1, G_pf2, G_dpf2, eta_star, and crossover_point) from the frequency sweep data if present.
    - **`'flow_step'`**: Contains rheological parameters (eta_0, eta_inf, K, n, error, and eta) from the flow step data if present.
    - `**'cox_merz'**`: Contains the viscosity (eta) and complex viscosity (eta_star) obtained from the Cox-Merz analysis if both frequency sweep and flow step data are present.

### Behavior

1. It reads the experimental data for the given sample ID (sid) from the Excel file specified by the **`df_ed`** parameter and stores it in the DataFrame **`df_ed`**.
2. The function performs various analyses based on the presence of specific columns in the DataFrame:
    - If 'time (min)' column is present, it calls the **`time_sweep_data_analysis()`** function to analyze the time sweep data and stores the mean and standard deviation values in the `**'time_sweep'**` dictionary entry.
    - If 'ang. Frequency (rad/s)' column is present, it calls the **`frequency_sweep_data_analysis()`** function to analyze the frequency sweep data and stores the rheological parameters in the **`'frequency_sweep'`** dictionary entry.
    - If 'shear rate (1/s)' column is present, it calls the **`flow_step_data_analysis()`** function to analyze the flow step data and stores the rheological parameters in the `**'flow_step'**` dictionary entry.
    - If both 'ang. Frequency (rad/s)' and 'shear rate (1/s)' columns are present, it calls the **`cox_merz_rule()`** function to perform Cox-Merz analysis and stores the results in the `**'cox_merz'**` dictionary entry.
3. If any specific type of data is missing, a message indicating its absence will be printed to the console.
4. The function returns the dictionary containing the analysis results for the given sample ID.

### Calling Example

Via the following example command the function loads the rheological primary data of the sample 57 from "Experimental_Data.xlsx" Excel database, performs its complete rheological analysis, prints a summary of them and returns them as a dictionary.

`**analysis_results = sample_analysis(snum=57, df_ed="Experimental_Data.xlsx")**`

---

# Chapter 6 - Database Filler

## Function: **append_samples_to_final_database(start_row_n, database_file="Database.xlsx", experiment_data_file="Experimental_Data.xlsx", analysis_data_file="Statistical_Analysis_Database.xlsx")**

### Description

This function loads an existing database file, processes the data for new samples starting from a specified sample number, and stores the analysis results back into the database. The new samples’ rheological data are extracted from the "Experimental_Data.xlsx" file located in the specified folder path. The database is updated with the analysis results for each new sample.

### Parameters

- **`start_row_n`** (int): The sample number from which to start the analysis. It indicates the number of the first new sample to be processed.
- **`database_file`** (str, optional): The filename of the database Excel file. The default value is "Database.xlsx".
- **`experiment_data_file`** (str, optional): The filename of the Excel file containing the experiment data for the new samples. The default value is "Experimental_Data.xlsx".
- `**analysis_data_file**` (str, optional): Name of the Excel file to be updated. Default value: "Statistical_Analysis_Database.xlsx".

### Returns

- `**result**` (DataFrame): The updated database with the analysis results. The DataFrame includes data for both the existing samples from the original database and the new samples from the experiment data file.

### Behavior

1. The function starts by converting the **`start_row_n`** parameter to a string to be used in constructing the sample ID for the first new sample.
2. It loads the existing database file specified by **`database_file`** into a DataFrame called **`database`**.
3. The function sets the "ID" column as the index of the DataFrame and removes any duplicates, keeping the first occurrence of each sample.
4. Certain columns that are not needed for analysis are dropped from the **`database`** DataFrame.
5. The resulting **`database`** DataFrame is printed to the console.
6. A new DataFrame called **`sub_database`** is created by slicing the original **`database`** DataFrame to select only the rows after the start row (i.e., the new samples).
7. The function iterates through each ID (row) in the **`sub_database`** DataFrame to process and analyze each new sample.
8. For each new sample, it calls the **`sample_analysis()`** function to perform the analysis and store the results in the **`analysis_results`** dictionary.
9. If the sample has time sweep data, the function updates the corresponding columns in the **`sub_database`** DataFrame with the mean and standard deviation values.
10. If the sample has frequency sweep data, the function updates the corresponding columns in the **`sub_database`** DataFrame with various rheological parameters.
11. If the sample has flow step data, the function updates the corresponding columns in the **`sub_database`** DataFrame with rheological parameters.
12. The **`sub_database`** DataFrame is printed for each new sample to the console.
13. After processing all new samples, the function concatenates the **`sub_database`** DataFrame with the existing database and stores the result in the **`result`** DataFrame.
14. The **`result`** DataFrame is written to the **`analysis_data_file`** Excel file without including an index.
15. Finally, the **`result`** DataFrame is returned, containing the updated database with the analysis results for both existing and new samples.

### Calling Example

Via the following example command the function loads all necessary database files ("Database.xlsx" and "Experimental_Data.xlsx"), performs the rheological analysis of all new samples starting from the sample 60, and stores the results in the "Statistical_Analysis_Database.xlsx" Excel database.

`**append_samples_to_final_database(start_row_n=60, database_file="Database.xlsx", experiment_data_file="Experimental_Data.xlsx", analysis_data_file="Statistical_Analysis_Database.xlsx")**`

---

# Chapter 7 - Technical Report Generator

## Function: **create_sample_report(snum, database_file="Database.xlsx", analysis_data_file="Statistical_Analysis_Database.xlsx", txt_file="report_template.txt", t_start=0.5, t_finish=5)**

### Description

This function generates a technical report for a specific sample identified by the given sample number. The report includes information from various sources, such as the database file, statistical analysis data file, and a template text file containing formatted variables and values.

### Parameters

- `**snum**` (int): The sample ID number for which the report is generated.
- **`database_file`** (str, optional): The filename of the database Excel file. The default value is "Database.xlsx".
- `**analysis_data_file**` (str, optional): The filename of the Excel file containing the statistical analysis data. The default value is "Statistical_Analysis_Database.xlsx".
- `**txt_file**` (str, optional): The filename of the text file serving as a report template. The default value is "report_template.txt".
- `**t_start**` (float, optional): The starting time in minutes for data analysis in the Time Sweep test. The default value is 0.5.
- **`t_finish`** (float, optional): The ending time in minutes for data analysis in the Time Sweep test. The default value is 5.

### Returns

- None: The function generates a technical report in PDF format and saves it as "HSF_{sid}*Report*{current_date}.pdf", where **`{sid}`** is the sample ID and **`{current_date}`** is the current date in "dd_mm_yyyy" format.

### Behavior

1. The function starts by constructing the sample ID (**`sid`**) using the given sample number (**`snum`**).
2. It loads the **`database_file`** and the **`analysis_data_file`** into two separate DataFrames (**`database`** and **`statistical_database`**, respectively).
3. The function extracts various information about the sample from the **`database`** and **`statistical_database`**, such as sampling date, gender, age, joint, condition, total volume, color, transparency, texture, and various test results from the analysis data.
4. It loads data from the **`report_template.txt`** file into a dictionary (**`variables`**) containing variables and their corresponding values. These variables are used to format the information in the report.
5. The function sets up the basic report information, including author, supervisor, today's date, and file name.
6. It creates different sections in the report, such as sample information, sample description, analysis, and results.
7. For each section, the function adds tables and figures to the report, along with the relevant data and text retrieved from the database and statistical analysis files.
8. The function saves the generated report as a PDF file named "HSF_{sid}*Report*{current_date}.pdf", where **`{sid}`** is the sample ID and **`{current_date}`** is the current date in "dd_mm_yyyy" format.

### Calling Example

Via the following example command the function loads the necessary sample’s 57 data from "Database.xlsx" and "Statistical_Analysis_Database.xlsx" Excel databases, as well as from "report_template.txt"txt file and creates the technical report of the sample’s analysis results.

`**create_sample_report(snum=57, database_file="Database.xlsx", analysis_data_file="Statistical_Analysis_Database.xlsx", txt_file="report_template.txt")**`

---

# Chapter 8 - Preprocessing Data

## Helper Function: **calculate_deviation(col1, col2, dataframe)**

### Description

This function calculates the deviation between two columns of a given DataFrame. It is particularly useful for comparing and analyzing the difference or variation between two sets of values within a dataset.

### Parameters

- `**col1**` (str): The name of the first column for which the deviation needs to be calculated.
- **`col2`** (str): The name of the second column for which the deviation needs to be calculated.
- `**dataframe**` (DataFrame): The DataFrame containing the two columns for deviation calculation.

<aside>
💡 The dataframe parameter should have the value of **`database`**, which refers to the DataFrame variable **`database`** of the `**preprocess_data()**` function.

</aside>

### Returns

- pandas Series: A pandas Series containing the deviation values calculated between the two specified columns. The Series will have the same length as the input DataFrame, and each element represents the deviation for the corresponding rows of **`col1`** and **`col2`**.

### Behavior

1. The function takes two column names, **`col1`** and **`col2`**, as input, along with an optional parameter **`dataframe`** that defaults to the global DataFrame **`database`**.
2. It calculates the deviation between the two columns using the formula: **`deviation = abs(dataframe[col1] - dataframe[col2]) / ((dataframe[col1] + dataframe[col2]) / 2)`**.
3. The result is a Series containing the deviation values, which is returned as the output.

## Function: **preprocess_data(primary_data_file="Statistical_Analysis_Database.xlsx")**

### Description

This function preprocesses the primary data contained in an Excel file by performing filtering and modifications to the data. It aims to handle missing or incorrect data, calculate deviations between certain columns, and filter out experiments that deviate significantly from expected values.

### Parameters

- `**primary_data_file**` (str, optional): The filename of the Excel file containing the primary data. The default value is "Statistical_Analysis_Database.xlsx".

### Returns

- `**database**` (DataFrame): A new DataFrame with the preprocessed data.

### Behavior

1. The function starts by loading the primary data from the Excel file specified by **`primary_data_file`** into a DataFrame named **`database`**, with the "ID" column set as the index.
2. It addresses missing values in the "Time Sweep G' average (Pa)" and "Time Sweep G'' average (Pa)" columns by filling them with the corresponding values from the "Frequency Sweep G' at 3.142 rad/s (Pa)" and "Frequency Sweep G'' at 3.142 rad/s (Pa)" columns, respectively.
3. The function filters out values in the "Cross Over Point (rad/s)" column that are larger than 15 and replaces them with NaN values. Additionally, it filters out values in certain columns, such as "Zero-rate Viscosity (Pa.s)", "Infinite-rate Viscosity (Pa.s)", "Consistency (s)", "Rate Index (-)", and "Standard Error (-)", that are greater than 50, less than 0.001, or outside certain thresholds, and sets them to NaN.
4. The function defines an internal helper function, **`calculate_deviation()`**, that takes two column names and computes the deviation between their values in the **`database`** DataFrame. The calculated deviations are then added to the DataFrame as new columns.
5. Using the calculated deviations, the function filters out experiments that deviate more than 20% in certain columns ("Frequency Sweep G' at 0.68 rad/s (Pa)", "Frequency Sweep G'' at 0.68 rad/s (Pa)", "Frequency Sweep G' at 3.142 rad/s (Pa)", "Frequency Sweep G'' at 3.142 rad/s (Pa)", "Frequency Sweep G' at 14.58 rad/s (Pa)", "Frequency Sweep G'' at 14.58 rad/s (Pa)", "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)", "Cross Over Point (rad/s)") and sets their values to NaN. Similarly, values in certain other columns ("Zero-rate Viscosity (Pa.s)", "Infinite-rate Viscosity (Pa.s)", "Consistency (s)", "Rate Index (-)", "Standard Error (-)", "Flow Step Viscosity at 3.162 1/s (Pa.s)") that deviate more than 20% are filtered and set to NaN.
6. The function calculates the "tan(delta)" values for specific frequencies using various columns and adds them as new columns in the DataFrame.
7. Finally, the function returns the preprocessed DataFrame, **`database`**, containing the modified and filtered data.

## Function: **apply_logarithm(df, columns_to_log)**

### Description

This function applies the logarithm (base 10) transformation to specified columns of the given DataFrame. The logarithm transformation is commonly used to compress large numeric ranges and reduce the impact of extreme values, making the data more amenable for analysis or visualization.

### Parameters

- `**df**` (DataFrame): The input DataFrame to be transformed.
- `**columns_to_log**` (list of str): A list containing the names of the columns that will undergo the logarithm transformation.

### Returns

- `**df**` (DataFrame): A new DataFrame with the specified columns logarithmically transformed.

### Behavior

1. The function takes a copy of the input DataFrame **`df`** to avoid modifying the original DataFrame.
2. It applies the logarithm (base 10) to each value in the columns specified in the **`columns_to_log`** list.
3. To avoid issues with values that might be zero or negative (which are not valid for the logarithm operation), the function adds 1 to each value before applying the logarithm. This ensures that all values are positive.
4. The logarithmically transformed values are then assigned back to the corresponding columns in the DataFrame.
5. The modified DataFrame with the logarithmically transformed columns is returned as the output.

<aside>
💡 It is assumed that the columns specified in **`columns_to_log`** contain numerical data, and the function will raise an error if non-numeric columns or columns with invalid data are included in the list.

</aside>

## Function: **prepare_dataframe(df, id_vars, value_vars, replacements=None)**

### Description

This function prepares a DataFrame for plotting by performing the following steps: melting, dropping rows with NaN (Not a Number) values, and applying replacements to variable names if specified. This preparation is particularly useful when working with data that needs to be transformed from wide format to long format for plotting.

### Parameters:

- `**df**` (DataFrame): The input DataFrame that needs to be prepared for plotting.
- `**id_vars**` (str or list of str): The column(s) to use as identifier variables when melting the DataFrame. These columns will be retained as they are during the melting process.
- `**value_vars**` (str or list of str): The column(s) to melt and use as value variables when transforming the DataFrame to long format. These columns will be combined into two new columns: one for the variable names and another for the corresponding values.
- `**replacements**` (dict, optional): A dictionary containing replacement values for specific variable names. The keys of the dictionary are the original variable names to be replaced, and the values are the new variable names. This parameter is optional and has a default value of None.

### Returns:

- `**plot**` (DataFrame): A new DataFrame prepared for plotting with the specified columns in long format.

### Behavior:

1. The function first performs the melting operation on the input DataFrame **`df`**. It uses the **`id_vars`** and **`value_vars`** parameters to reshape the DataFrame from wide format to long format. The melted DataFrame will have two new columns, "Variable" and "Value," where "Variable" contains the names of the original columns specified in **`value_vars`**, and "Value" contains the corresponding values from those columns.
2. Next, the function drops rows from the melted DataFrame where the "Value" is NaN. This step removes any missing or invalid data that could interfere with plotting or analysis.
3. A copy of the resulting DataFrame is created to avoid modifying the original DataFrame.
4. If the **`replacements`** parameter is provided (not None), the function performs replacements on the "Variable" column according to the specified dictionary. Any original variable names present as keys in the dictionary will be replaced with the corresponding values specified as replacements.
5. The modified DataFrame with the melted, cleaned, and potentially renamed columns is returned as the output.

## Function: **legend_prepare_dataframe(df, A, B)**

### Description

This function prepares a DataFrame for legend replacement by mapping specified values to new values in the DataFrame.

### Parameters:

- `**df**` (pd.DataFrame): The input DataFrame that requires legend replacement.
- `**A**` (str): The replacement value for the original value 'yes' found in the DataFrame.
- `**B`** (str): The replacement value for the original value 'no' found in the DataFrame.

### Returns:

- `**DataFrame**`: A new DataFrame prepared for legend replacement with the specified replacements applied.

### Behavior:

1. The function performs replacement operations on the input DataFrame **`df`**. Specifically, it replaces occurrences of 'yes' with the value specified by **`A`**, and occurrences of 'no' with the value specified by **`B`**.
2. The modified DataFrame with the replacements applied is returned as the output.

### Calling Example

Via the following example code the primary data from the "Statistical_Analysis_Database.xlsx" Excel database are preprocessed and prepared for further analysis. 

1. The data are loaded from "Statistical_Analysis_Database.xlsx" Excel database and via the `**preprocess_data()**` helper function they are filtered and cleaned up.
2. They are categorised into dataframes with subsets of the total database with specific characteristics each time, such as samples’ from specific joint or with specific condition.
3. Some of these subsets are also logarithmically transformed via $log(var+1)$ equation with the use of `**apply_logarithm()**` helper function.
4. The DataFrames are prepared for plotting by melting, dropping NaN values, and applying replacements to variable names.
5. To some of these data

```python
database = preprocess_data(primary_data_file="Statistical_Analysis_Database.xlsx")

# Filter and clean dataframes based on certain conditions
clean_df = database[(database["Joint"] == "knee") & (database["Blood"] == "no") & (database["Tissue or Clot in Test"] == "no")]
clean_df = clean_df.drop(columns=["Joint", "Blood", "Clot", "Tissue", "Tissue or Clot in Test", 'Storage in freezer', 'COVID 19 now', 'COVID 19', 'Vaccined COVID 19'])
OA_df = database[(database["Joint"] == "knee") & (database["Condition"] == "oa") & (database["Blood"] == "no") & (database["Tissue or Clot in Test"] == "no")]
OA_df = OA_df.drop(columns=["Joint", "Clot", "Tissue", "Tissue or Clot in Test", 'COVID 19 now', 'COVID 19', 'Vaccined COVID 19'])
healthy_df = database[(database["Joint"] == "knee") & (database["Condition"] == "healthy") & (database["Blood"] == "no") & (database["Tissue or Clot in Test"] == "no")]
healthy_df = healthy_df.drop(columns=["Joint", "Clot", "Tissue", "Tissue or Clot in Test", 'COVID 19 now', 'COVID 19', 'Vaccined COVID 19'])
clean_df = pd.concat([healthy_df, OA_df], axis=0, ignore_index=True)

OA_blood_df = database[(database["Joint"] == "knee") & (database["Condition"] == "oa") & (database["Blood"] == "yes") & (database["Tissue or Clot in Test"] == "no")]
OA_blood_df = OA_blood_df.drop(columns=["Joint", "Clot", "Tissue", "Tissue or Clot in Test", 'COVID 19 now', 'COVID 19', 'Vaccined COVID 19'])
OA_total_df = pd.concat([OA_blood_df, OA_df], axis=0, ignore_index=True)
healthy_blood_df = database[(database["Joint"] == "knee") & (database["Condition"] == "healthy") & (database["Blood"] == "yes") & (database["Tissue or Clot in Test"] == "no")]
healthy_blood_df = healthy_blood_df.drop(columns=["Joint", "Clot", "Tissue", "Tissue or Clot in Test", 'COVID 19 now', 'COVID 19', 'Vaccined COVID 19'])
healthy_total_df = pd.concat([healthy_blood_df, healthy_df], axis=0, ignore_index=True)
total_df = pd.concat([healthy_total_df, OA_total_df], axis=0, ignore_index=True)
    
OA_storage_df = OA_df.copy().reset_index(drop=True)
OA_male_df = OA_df.copy().loc[database["Gender"] == "male"].reset_index(drop=True)
OA_female_df = OA_df.copy().loc[database["Gender"] == "female"].reset_index(drop=True)

columns_to_log = [
    "Frequency Sweep G' at 0.68 rad/s (Pa)",
    "Frequency Sweep G'' at 0.68 rad/s (Pa)",
    "Time Sweep G' average (Pa)",
    "Time Sweep G'' average (Pa)",
    "Frequency Sweep G' at 14.58 rad/s (Pa)",
    "Frequency Sweep G'' at 14.58 rad/s (Pa)",
    "Flow Step Viscosity at 3.162 1/s (Pa.s)",
    "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)",
    "Cross Over Point (rad/s)",
    "tan(delta) at 0.68 rad/s",
    "tan(delta) at 3.142 rad/s",
    "tan(delta) at 14.58 rad/s"
]

OA_df_log = apply_logarithm(OA_df.copy(), columns_to_log)
healthy_df_log = apply_logarithm(healthy_df.copy(), columns_to_log)
clean_df_log = pd.concat([healthy_df_log, OA_df_log], axis=0, ignore_index=True)

OA_total_df_log = apply_logarithm(OA_total_df.copy(), columns_to_log)
healthy_total_df_log = apply_logarithm(healthy_total_df.copy(), columns_to_log)
total_df_log = pd.concat([healthy_total_df_log, OA_total_df_log], axis=0, ignore_index=True)

OA_blood_df_log = apply_logarithm(OA_blood_df.copy(), columns_to_log)
OA_storage_df_log = apply_logarithm(OA_storage_df.copy(), columns_to_log)
    
OA_male_df_log = apply_logarithm(OA_male_df.copy(), columns_to_log)
OA_female_df_log = apply_logarithm(OA_female_df.copy(), columns_to_log)

# Define the value_vars and replacements for each category
value_vars1 = ["Frequency Sweep G' at 0.68 rad/s (Pa)", "Frequency Sweep G'' at 0.68 rad/s (Pa)",
               "Time Sweep G' average (Pa)", "Time Sweep G'' average (Pa)",
               "Frequency Sweep G' at 14.58 rad/s (Pa)", "Frequency Sweep G'' at 14.58 rad/s (Pa)"]
replacements1 = {
    "Frequency Sweep G' at 0.68 rad/s (Pa)": "G' at 0.68 rad/s",
    "Frequency Sweep G'' at 0.68 rad/s (Pa)": "G'' at 0.68 rad/s",
    "Frequency Sweep G' at 14.58 rad/s (Pa)": "G'' at 14.58 rad/s",
    "Frequency Sweep G'' at 14.58 rad/s (Pa)": "G' at 14.58 rad/s",
    "Time Sweep G' average (Pa)": "G' at 3.142 rad/s",
    "Time Sweep G'' average (Pa)": "G'' at 3.142 rad/s"
}

value_vars2 = ["Flow Step Viscosity at 3.162 1/s (Pa.s)", "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)"]
replacements2 = {
    "Flow Step Viscosity at 3.162 1/s (Pa.s)": "n",
    "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)": "|n*|"
}

value_vars3 = ["Cross Over Point (rad/s)"]
replacements3 = {
    "Flow Step Viscosity at 3.162 1/s (Pa.s)": "n",
    "Cross Over Point (rad/s)": "Cross Over Point"
}

value_vars4 = ["tan(delta) at 0.68 rad/s", "tan(delta) at 3.142 rad/s", "tan(delta) at 14.58 rad/s"]
replacements4 = {
    "tan(delta) at 0.68 rad/s": "tan(delta) at 0.68 rad/s",
    "tan(delta) at 3.142 rad/s": "tan(delta) at 3.142 rad/s",
    "tan(delta) at 14.58 rad/s": "tan(delta) at 14.58 rad/s"
}

# Prepare DataFrames for plotting and legend replacement
clean_osc = prepare_dataframe(clean_df, "Condition", value_vars1, replacements1)
clean_n = prepare_dataframe(clean_df, "Condition", value_vars2, replacements2)                                 
clean_cop = prepare_dataframe(clean_df, "Condition", value_vars3, replacements3)
clean_tand = prepare_dataframe(clean_df, "Condition", value_vars4, replacements4)

total_osc = prepare_dataframe(total_df, "Condition", value_vars1, replacements1)
total_n = prepare_dataframe(total_df, "Condition", value_vars2, replacements2)                                  
total_cop = prepare_dataframe(total_df, "Condition", value_vars3, replacements3)
total_tand = prepare_dataframe(total_df, "Condition", value_vars4, replacements4)

OA_total_osc = prepare_dataframe(OA_total_df, "Blood", value_vars1, replacements1)
OA_total_osc = legend_prepare_dataframe(OA_total_osc, "With", "Without")
OA_total_n = prepare_dataframe(OA_total_df, "Blood", value_vars2, replacements2)
OA_total_n = legend_prepare_dataframe(OA_total_n, "With", "Without")
OA_total_cop = prepare_dataframe(OA_total_df, "Blood", value_vars3, replacements3)
OA_total_cop = legend_prepare_dataframe(OA_total_cop, "With", "Without")
OA_total_tand = prepare_dataframe(OA_total_df, "Blood", value_vars4, replacements4)
OA_total_tand = legend_prepare_dataframe(OA_total_tand, "With", "Without")

OA_storage_osc = prepare_dataframe(OA_storage_df, "Storage in freezer", value_vars1, replacements1)
OA_storage_osc = legend_prepare_dataframe(OA_storage_osc, "Frozen", "Not Frozen")
OA_storage_n = prepare_dataframe(OA_storage_df, "Storage in freezer", value_vars2, replacements2)
OA_storage_n = legend_prepare_dataframe(OA_storage_n, "Frozen", "Not Frozen")
OA_storage_cop = prepare_dataframe(OA_storage_df, "Storage in freezer", value_vars3, replacements3)
OA_storage_cop = legend_prepare_dataframe(OA_storage_cop, "Frozen", "Not Frozen")
OA_storage_tand = prepare_dataframe(OA_storage_df, "Storage in freezer", value_vars4, replacements4)
OA_storage_tand = legend_prepare_dataframe(OA_storage_tand, "Frozen", "Not Frozen")

gender_OA_total_osc = prepare_dataframe(OA_total_df, "Gender", value_vars1, replacements1)
gender_OA_total_n = prepare_dataframe(OA_total_df, "Gender", value_vars2, replacements2)
gender_OA_total_cop = prepare_dataframe(OA_total_df, "Gender", value_vars3, replacements3)
gender_OA_total_tand = prepare_dataframe(OA_total_df, "Gender", value_vars4, replacements4)
```

---

# Chapter 9 - Statistical Analyser

## Function: **statistics(data1, data2, column_names, alpha=0.05)**

### Description

This function performs basic statistics calculations (count, mean value, standard deviation, max and min value) and an independent two-sample t-test between two sets of data for each specified column. It is useful for comparing the means of two samples and determining if there is a significant difference between them.

### Parameters

- `**data1**` (DataFrame): The first DataFrame containing the first set of data for comparison.
- `**data2**` (DataFrame): The second DataFrame containing the second set of data for comparison.
- `**column_names**` (list): A list of column names in both DataFrames on which the t-test will be performed.
- `**alpha**` (float, optional): The significance level for the hypothesis test. It determines the threshold for accepting or rejecting the null hypothesis. The default value is 0.05, which corresponds to a 5% significance level.

### Returns

- `**results_df**` (DataFrame): A pandas DataFrame containing the results of the basic statistics and the t-test for each specified column. The DataFrame includes the following columns:
    - `**'Column'**`: The name of the column for which the basic statistics calculations and t-test were performed.
    - `**'Count 1'**`: The number of column elements of first input DataFrame.
    - `**'Mean 1'**`: The mean value of column elements of first input DataFrame.
    - `**'Std 1'**`: The standard deviation of column elements of first input DataFrame.
    - `**'Max 1'**`: The max value of column elements of first input DataFrame.
    - `**'Min 1'**`: The min value of column elements of first input DataFrame.
    - `**'Count 2'**`: The number of column elements of second input DataFrame.
    - `**'Mean 2'**`: The mean value of column elements of second input DataFrame.
    - `**'Std 2'**`: The standard deviation of column elements of second input DataFrame.
    - `**'Max 2'**`: The max value of column elements of second input DataFrame.
    - `**'Min 2'**`: The min value of column elements of second input DataFrame.
    - `**'t-statistic'**`: The calculated t-statistic for the t-test.
    - `**'p-value'**`: The p-value resulting from the t-test.
    - `**'Hypothesis'**`: The hypothesis decision, indicating whether to 'Reject' or 'Accept' the null hypothesis based on the p-value and the specified alpha level.

### Behavior

1. The function takes two DataFrames, **`data1`** and **`data2`**, which represent the two sets of data to compare, along with a list of **`column_names`** specifying the columns in both DataFrames for which the t-test will be performed.
2. For each column specified in **`column_names`**, the function extracts the non-null samples from both DataFrames.
3. It checks if both samples have non-zero element number (greater than 0) and calculates the basic statistics.
4. It checks if both samples have non-zero variance (greater than 0) to ensure the t-test is valid. If either sample has zero variance, the t-test cannot be performed, and the 't-statistic' and 'p-value' are set to NaN, and the 'Hypothesis' is left empty.
5. If both samples have non-zero variance, the function calculates the t-statistic and p-value for the t-test using **`scipy.stats.ttest_ind`** function, which performs a two-sample t-test assuming equal variances.
6. The p-value is then compared with the specified **`alpha`** level to make a decision on whether to 'Reject' or 'Accept' the null hypothesis. If the p-value is less than alpha, the null hypothesis is rejected, indicating that there is a significant difference between the two sample means. Otherwise, the null hypothesis is accepted, suggesting that there is no significant difference.
7. The function stores the results for each column in a list of dictionaries, with each dictionary representing the result for a specific column. The results are then converted into a DataFrame named **`results_df`**, and the DataFrame is returned as the output.

<aside>
💡 The null hypothesis (H0) of the t-test is that there is no significant difference between the means of the two samples. The alternative hypothesis (H1) is that there is a significant difference.

</aside>

### Calling Example

Via the following example code an independent two-sample t-test between two sets of data, logarithmically transformed OA and healthy clean samples. The t and p values, as well as the rejection or acceptance of the null hypothesis are saved in a DataFrame `**results_df**`, and displayed. The output displayed DataFrame of this particular example is presented bellow the coding cell.

```python
# Assuming you have DataFrames called 'OA_df_log' and 'healthy_df_log'
column_names = [
    "Frequency Sweep G' at 0.68 rad/s (Pa)",
    "Frequency Sweep G'' at 0.68 rad/s (Pa)",
    "Time Sweep G' average (Pa)",
    "Time Sweep G'' average (Pa)",
    "Frequency Sweep G' at 14.58 rad/s (Pa)",
    "Frequency Sweep G'' at 14.58 rad/s (Pa)",
    "Flow Step Viscosity at 3.162 1/s (Pa.s)",
    "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)",
    "Cross Over Point (rad/s)",
    "tan(delta) at 0.68 rad/s",
    "tan(delta) at 3.142 rad/s",
    "tan(delta) at 14.58 rad/s"
]

# Perform t-tests and display results
results_df = perform_t_test(healthy_df_log, OA_df_log, column_names)
display(results_df)
```

![Screenshot 2023-08-03 221713.png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/Screenshot_2023-08-03_221713.png)

## Helper Function: **categorize(df, col, limit, big_var="control")**

### Description

This function categorizes the data in the DataFrame based on a specified column and a given limit (threshold). It allows for the assignment of categories such as "True Positive (TP)", "True Negative (TN)", "False Positive (FP)", and "False Negative (FN)" based on the comparison of the column values with the specified limit.

### Parameters

- `**df**` (DataFrame): The DataFrame containing the data to be categorized.
- `**col**` (str): The name of the column in the DataFrame used for categorization.
- `**limit**` (float): The threshold value for the categorization. Values above or below this limit will be assigned to different categories depending on the **`big_var`** parameter.
- **`big_var`** (str, optional): The variable used to determine whether to consider values above or below the limit as "positive". The default value is "control", which means that values below the limit will be considered "positive". If set to any other value, values above the limit will be considered "positive".

### Returns

- `**df**` (DataFrame): The modified DataFrame with a new column named "Category" containing the categories assigned based on the comparison with the specified limit.

### Behavior

1. The function first drops any rows containing NaN values in the specified column **`col`** to ensure valid comparisons.
2. The DataFrame's index is then reset to ensure consecutive indexing.
3. For each row in the DataFrame, the function checks the value of the **`big_var`** parameter and the condition in the "Condition" column. Based on these factors and the comparison of the value in the specified **`col`** with the **`limit`**, the function assigns the corresponding category to the "Category" column as follows:
    - If **`big_var`** is "control" and the row's "Condition" is "oa", and the value in **`col`** is less than **`limit`**, the category is "TP" (True Positive). Otherwise, the category is "FN" (False Negative).
    - If **`big_var`** is "control" and the row's "Condition" is not "oa", and the value in **`col`** is less than **`limit`**, the category is "FP" (False Positive). Otherwise, the category is "TN" (True Negative).
    - If **`big_var`** is not "control" and the row's "Condition" is "oa", and the value in **`col`** is greater than **`limit`**, the category is "TP" (True Positive). Otherwise, the category is "FN" (False Negative).
    - If **`big_var`** is not "control" and the row's "Condition" is not "oa", and the value in **`col`** is greater than **`limit`**, the category is "FP" (False Positive). Otherwise, the category is "TN" (True Negative).
4. The modified DataFrame is returned as the output.

## Helper Function: **count_values(df)**

### Description

This function counts the occurrences of each category in the "Category" column of the DataFrame. It provides the counts for the categories "TN" (True Negative), "TP" (True Positive), "FN" (False Negative), and "FP" (False Positive).

### Parameters

- `**df**` (DataFrame): The DataFrame containing the "Category" column.

### Returns

- `**counts**` (dict): A dictionary containing the counts of each category in the format {"Category": count}.

### Behavior

1. The function initializes a list of categories, including "TN", "TP", "FN", and "FP".
2. It then counts the occurrences of each category in the "Category" column of the DataFrame **`df`** and stores the counts in a dictionary.
3. The dictionary is returned as the output.

## Function: **biomarker_validation(df, biomarkers_info)**

### Description

This function performs biomarker validation by categorizing data and calculating various metrics for each specified biomarker. It allows for the comparison of biomarker data against specific thresholds and provides metrics such as Sensitivity, Specificity, Accuracy, and Youden's Index.

### Parameters

- `**df**` (DataFrame): The DataFrame containing the biomarker data.
- `**biomarkers_info**` (list): A list of lists containing biomarker information for validation. Each list in the format: [Biomarker_Name, Column_Name, Threshold, Category], where:
    - `**Biomarker_Name**` (str): The name of the biomarker.
    - `**Column_Name**` (str): The name of the column in the DataFrame containing the biomarker data.
    - `**Threshold**` (float): The threshold value for categorization of the biomarker data.
    - `**Category**` (str): The variable used to determine whether values above or below the threshold are considered "positive". Options are "control" (values below threshold are "positive") or any other value (values above threshold are "positive").

### Returns

- `**biomarker_df**` (DataFrame): A DataFrame containing biomarker validation metrics for each biomarker. The DataFrame includes the following columns:
    - **`"Biomarker"`**: The name of the biomarker.
    - `**"TN"**`: Count of True Negative cases.
    - **`"TP"`**: Count of True Positive cases.
    - `**"FN"**`: Count of False Negative cases.
    - `**"FP"**`: Count of False Positive cases.
    - `**"Threshold"**`: The threshold value used for biomarker validation.
    - `**"Sensitivity"**`: Sensitivity metric calculated as TP / (TP + FN).
    - `**"Specificity"**`: Specificity metric calculated as TN / (TN + FP).
    - `**"Accuracy"**`: Accuracy metric calculated as (TP + TN) / (TP + TN + FP + FN).
    - `**"Youden's Index"**`: Youden's Index metric calculated as Sensitivity + Specificity - 1.

### Behavior

1. The function initializes an empty DataFrame named **`biomarker_df`** with columns for storing biomarker validation metrics.
2. For each biomarker specified in the **`biomarkers_info`** list:
    - A copy of the original DataFrame **`df`** is created and assigned to **`biomarkers_data`**.
    - The biomarker name, threshold value, and category are extracted from the **`biomarkers_info`** list for the current biomarker.
    - The function **`categorize`** is called to categorize the data in **`biomarkers_data`** based on the biomarker information.
    - The function **`count_values`** is called to count the occurrences of each category in the "Category" column of **`biomarkers_data`**.
    - The counts of True Negative (TN), True Positive (TP), False Negative (FN), and False Positive (FP) are extracted from the returned dictionary.
    - A new row containing biomarker validation metrics for the current biomarker is created and appended to the **`biomarker_df`** DataFrame.
3. Sensitivity, Specificity, Accuracy, and Youden's Index are calculated and added as additional columns to **`biomarker_df`**.
4. The **`biomarker_df`** DataFrame with biomarker validation metrics is returned as the output.

### Calling Example

Via the following example code the biomarker validation is performed. The sample data from `**clean_df**` DataFrame are categorised with the particular threshold values, provided by the user in the `**biomarkers_info**` list, and the Key Performance Indicators (Sensitivity, Specificity, Accuracy, and Youden’s Index) are calculated, saved in a DataFrame `**biomarker_df**`, and displayed. The output displayed DataFrame of this particular example is presented bellow the coding cell.

```python
# Assuming you have a DataFrame called 'clean_df'
# Dictionary to store biomarker names and their corresponding columns, limits, and big_var
biomarkers_info = [
    ["G' at 0.68 rad/s", "Frequency Sweep G' at 0.68 rad/s (Pa)", 2.18, "control"],
    ["G'' at 0.68 rad/s", "Frequency Sweep G'' at 0.68 rad/s (Pa)", 1.88, "control"],
    ["G' at 3.142 rad/s", "Time Sweep G' average (Pa)", 4.34, "control"],
    ["G'' at 3.142 rad/s", "Time Sweep G'' average (Pa)", 2.58, "control"],
    ["G' at 14.58 rad/s", "Frequency Sweep G' at 14.58 rad/s (Pa)", 7.28, "control"],
    ["G'' at 14.58 rad/s", "Frequency Sweep G'' at 14.58 rad/s (Pa)", 3.06, "control"],
    ["Viscosity |n*| at 3.142 rad/s", "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)", 1.65, "control"],
    ["tan(delta) at 0.68 rad/s", "tan(delta) at 0.68 rad/s", 0.88, "target"],
    ["tan(delta) at 3.142 rad/s", "tan(delta) at 3.142 rad/s", 0.65, "target"],
    ["tan(delta) at 14.58 rad/s", "tan(delta) at 14.58 rad/s", 0.48, "target"]
]

biomarker_df = biomarker_validation(clean_df, biomarkers_info)

display(biomarker_df)
```

![Screenshot 2023-08-01 115311.png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/Screenshot_2023-08-01_115311.png)

---

# Chapter 10 - Plotting

## **create_custom_boxplot(data, x_label, y_label, x_ticklabels, hue, hue_order, legend_labels, width=0.8, dodge=True, yA=0, yB=None)**

### Description

This function creates a custom box plot using Seaborn, a popular Python data visualization library. The box plot displays the distribution of data across different categories and provides visual insights into the central tendency, spread, and potential outliers of each category.

### Parameters

- **`data`** (DataFrame): The DataFrame containing the data to be plotted.
- `**x_label**` (str): Label for the x-axis, representing the variable or feature on the x-axis.
- `**y_label**` (str): Label for the y-axis, representing the values of the variable being analyzed.
- `**x_ticklabels**` (list): List of tick labels for the x-axis, representing the labels of the different categories or groups displayed on the x-axis.
- `**hue**` (str): Grouping variable for categorical coloring. This variable is used to split the data into different groups based on its values and color the box plots accordingly.
- `**hue_order**` (list): Order of hue levels (grouping variable) for categorical coloring. It specifies the order in which the different levels of the hue variable should be displayed.
- `**legend_labels**` (list): Labels for the legend. These labels provide a custom representation for the different categories displayed in the legend of the box plot.
- `**width**` (float, optional): Width of the boxes. It determines the width of the boxes representing each category in the box plot. The default value is 0.8.
- `**dodge**` (bool, optional): When True, use a small positional jitter to avoid overlap when plotting hue levels. If set to False, the box plots for different hue levels may overlap. The default value is True.
- `**yA**` (int, optional): The lowest y-axis limit. It sets the lower limit for the y-axis values displayed in the plot. The default value is 0.
- `**yB**` (int, optional): The highest y-axis limit. It sets the upper limit for the y-axis values displayed in the plot. If set to None, there is no change in the y-axis limits. The default value is None.

### Returns

- `**None**`: The function does not return any value explicitly; It generates the custom box plot and displays it as an interactive plot.

### Behavior

1. The Seaborn theme "darkgrid" and a custom color palette are set to enhance the visual appearance of the box plot.
2. The function creates a box plot using the **`sns.boxplot`** method from Seaborn, with the data and various parameters specified in the function arguments.
3. The box plot displays the distribution of data for each category (specified by **`hue`**) along the x-axis and the corresponding values (specified by **`y_label`**) along the y-axis.
4. Each category is represented by a box, which indicates the interquartile range (IQR) and median of the data in that category.
5. Any data points beyond the whiskers are displayed as individual points, representing potential outliers.
6. The boxes are filled with a transparent color to distinguish the different categories visually.
7. The function customizes the plot by setting the x-axis and y-axis labels, adjusting the x-axis tick labels' rotation, and adding a legend with custom labels specified in **`legend_labels`**.
8. The function uses **`plt.show()`** to display the plot interactively.

### Calling Example

Via the following example code the 4 main box plots for data visualization purposes are generated. With these 4 box plots a comparison of the biomarkers’ values between OA and healthy clean samples is performed.  The function `**create_custom_boxplot()**` is called four times, each time with different arguments, such as different x and y variables and labels, legends, etc. The output plots of this particular example is presented bellow the coding cell.

```python
# Assuming you have DataFrames called 'clean_osc', 'clean_tand', 'clean_n', and 'clean_cop'
# Call the function with different data and labels
create_custom_boxplot(clean_osc, "", "G' και G'' (Pa)", ["G'-0.68 rad/s", "G''-0.68 rad/s", "G'-3.142 rad/s", "G''-3.142 rad/s", "G'-14.58 rad/s", "G''-14.58 rad/s"], 
                      hue="Condition", hue_order=['healthy', 'oa'], legend_labels=['Healthy', 'OA'], 
                      width=0.8, dodge=True, yA=0, yB=None)

create_custom_boxplot(clean_tand, "", "tan(δ)", ["0.68 rad/s", "3.142 rad/s", "14.58 rad/s"],
                      hue="Condition", hue_order=['healthy', 'oa'], legend_labels=['Healthy', 'OA'], 
                      width=0.8, dodge=True, yA=0, yB=None)

create_custom_boxplot(clean_n, "", "n and |n*| (Pa.s)", ["n", "|n*|"],
                      hue="Condition", hue_order=['healthy', 'oa'], legend_labels=['Healthy', 'OA'], 
                      width=0.8, dodge=True, yA=0, yB=None)

create_custom_boxplot(clean_cop, "", "Cross-over point (rad/s)", [""],
                      hue="Condition", hue_order=['healthy', 'oa'], legend_labels=['Healthy', 'OA'], 
                      width=0.2, dodge=True, yA=0, yB=None)
```

![download.png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/download.png)

![download (1).png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/download_(1).png)

![download (2).png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/download_(2).png)

![download (3).png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/download_(3).png)

---

# Chapter 11 - Monte Carlo Simulation

## **Function: multivariate_normal_sampling(dataframe, columns, scaled_factor=1)**

### **Description**

This function samples from a multivariate normal distribution based on specified columns of a given DataFrame. It calculates the mean vector and covariance matrix of the specified columns, optionally scales the standard deviation to create a more robust model, and generates samples using these parameters.

### **Parameters**

- **`dataframe`** (pd.DataFrame): The input DataFrame containing the data.
- **`columns`** (list): List of column names to sample from.
- **`scaled_factor`** (int, optional): A scaling factor to scale the standard deviation of the original data to create a more robust model. Default value is 1.

### **Returns**

- `**sampled_data**` (DataFrame): A DataFrame containing the sampled data.

### **Behavior**

1. The function first extracts the specified columns from the input DataFrame and drops rows with missing values.
2. It calculates the mean vector and covariance matrix of the selected columns.
3. The standard deviation of the covariance matrix is optionally scaled by the **`scaled_factor`** value.
4. Samples are generated from a multivariate normal distribution using the calculated mean vector and scaled covariance matrix.
5. The sampled values are stored in a new DataFrame with the original column names.
6. The function returns the DataFrame with the sampled data.

### Calling Example

Via the following example code a DataFrame with artificial samples is created. The artificial samples are produced with a multivariate Monte Carlo sampling technique. A part of the output DataFrame of this particular example is presented bellow the coding cell.

```python
# Assuming you have DataFrames called 'healthy_df_log' and 'OA_df_log'
# Specify the columns to sample
columns_to_sample = ["Frequency Sweep G' at 0.68 rad/s (Pa)",
                     "Frequency Sweep G'' at 0.68 rad/s (Pa)",
                     "Time Sweep G' average (Pa)",
                     "Time Sweep G'' average (Pa)",
                     "Frequency Sweep G' at 14.58 rad/s (Pa)",
                     "Frequency Sweep G'' at 14.58 rad/s (Pa)",
                     "Frequency Sweep Viscosity at 3.142 rad/s (Pa.s)"]

# Sample from multivariate normal distribution for healthy_df_log
healthy_artificial_df = multivariate_normal_sampling(healthy_df_log, columns_to_sample, scaled_factor=2)
healthy_artificial_df['Condition'] = 0

# Sample from multivariate normal distribution for OA_df_log
OA_artificial_df = multivariate_normal_sampling(OA_df_log, columns_to_sample, scaled_factor=2)
OA_artificial_df['Condition'] = 1

# Concatenate the sampled DataFrames for both conditions
artificial_df = pd.concat([healthy_artificial_df, OA_artificial_df], axis=0, ignore_index=True)

# Shuffle the rows randomly
artificial_df = artificial_df.reindex(np.random.permutation(artificial_df.index))

# Reset the index of the DataFrame
artificial_df = artificial_df.reset_index(drop=True)

# Display the resulting artificial DataFrame
display(artificial_df)
```

![Screenshot 2023-08-06 172152.png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/Screenshot_2023-08-06_172152.png)

---

# Chapter 12 - Machine Learning Models

## **Function: logistic_regression**(dataframe, columns)

### **Description**

This function performs logistic regression modeling on a given DataFrame using specified predictor variables. It trains the model, evaluates its performance using cross-validation, and performs ROC analysis to assess the model's ability to distinguish between classes.

### **Parameters**

- **`dataframe`** (pd.DataFrame): The input DataFrame containing the data.
- **`columns`** (list): List of column names to use as predictor variables.

### **Returns**

- `**cross_val_accuracy`** (float): The mean cross-validation accuracy of the trained model.

### **Behavior**

1. The function defines the predictor variables (**`X`**) and the response variable (**`y`**) from the input DataFrame.
2. It splits the dataset into training (60%) and testing (40%) sets using the **`train_test_split`** function.
3. An instance of the logistic regression model is instantiated.
4. The model is trained using the training data.
5. Cross-validation is performed using the **`cross_val_score`** function with 5-fold cross-validation, and the mean accuracy is calculated.
6. ROC curve metrics (fpr, tpr, auc) are computed using the **`predict_proba`** method of the trained model.
7. The ROC curve is plotted using Matplotlib, showing sensitivity against specificity.
8. The function returns the mean cross-validation accuracy of the trained model.

### Calling Example

Via the following example code a logistic regression machine learning model is trained with the artificial data produced via the Monte Carlo Simulation and used in order to predict the condition of other data. The output of this particular example is presented bellow the coding cell.

```python
# Assuming you have DataFrames called 'artificial_df'
# Specify the columns to use as predictor variables
columns_to_predict = ["Time Sweep G' average (Pa)",
                      "Time Sweep G'' average (Pa)"]

# Train, evaluate, and perform ROC analysis for the logistic regression model
mean_cross_val_accuracy = logistic_regression(artificial_df, columns_to_predict)

print("Mean Cross-Validation Accuracy:", mean_cross_val_accuracy)
```

![Screenshot 2023-08-06 172213.png](Rheological%20Analysis%20Toolbox%20caf04f0f4f2c4d30b31cbca9400580f0/Screenshot_2023-08-06_172213.png)

---
# Group 9, Project 3

**Team Members:** Austin Chun (Leader), Mackenzie Craig, Jackson Haiz

---

**Goal:** This file serves as an orientation to Project 3, providing all necessary files (code, data, and documentation) to understand the project's contents and reproduce its results.

## Repository Contents

This repository is structured to organize the project's data, scripts, and output clearly. Details for reproducing the results, the required software, and a map of the documentation are provided below.

### 1: Software and Platform Section

* **Type(s) of software used for the project:**
    * **Python** (Version 3.10 or higher)

* **Names of any add-on packages that need to be installed with the software:**
    The project relies on standard Python data science libraries. They can be installed using `pip`.
    * `pandas` (for data manipulation)
    * `numpy` (for numerical operations)
    * `scikit-learn` (for machine learning models)
    * `matplotlib` and/or `seaborn` (for visualization)
    * *We recommend using a virtual environment and installing all required packages via a `requirements.txt` file:*
        ```bash
        pip install -r requirements.txt
        ```

* **The platform (e.g., Windows, Mac, or Linux) you used:**
    * The project was developed and tested on a mix of **macOS** and **Windows 10**.

### 2: A Map of your documentation

The following outline illustrates the hierarchy of folders and files contained in the Project Folder:

```text
Project3_G9_DS_4001/
├── DATA/
│   ├── raw_data.csv          # The initial, unprocessed dataset.
│   └── cleaned_data.csv      # The final dataset after preprocessing and cleaning.
├── OUTPUT/
│   ├── final_model.pkl       # The serialized machine learning model object.
│   ├── results_summary.txt   # A text file summarizing key findings.
│   └── figure_1.png          # A key visualization/figure generated from the analysis.
├── SCRIPTS/
│   ├── 01_data_cleaning.ipynb    # Notebook for data ingestion and preprocessing.
│   ├── 02_analysis_and_model.py  # Main Python script for model training and evaluation.
│   └── 03_visualization.ipynb    # Notebook for generating project visuals.
├── LICENSE                     # MIT License for the project.
├── README.md                   # This file.
└── references                  # A plain text file listing all external data and literature sources.****
### 3: Instructions for Reproducing your Results

1.  **Clone the Repository:**
    Use Git to clone the repository to your local machine:
    ```bash
    git clone [https://github.com/austincychun/Project3_G9_DS_4001.git](https://github.com/austincychun/Project3_G9_DS_4001.git)
    cd Project3_G9_DS_4001
    ```

2.  **Set Up the Environment:**
    Ensure you have **Python (3.10+)** installed. Create and activate a virtual environment (recommended) and install the dependencies (assuming a `requirements.txt` file is present):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

3.  **Run the Data Processing Script:**
    Execute the data cleaning and feature engineering steps:
    ```bash
    python SCRIPTS/01_data_cleaning.ipynb # or run this notebook in a Jupyter environment
    ```
    *This will generate the `cleaned_data.csv` file in the `DATA` directory.*

4.  **Run the Main Analysis and Modeling Script:**
    Execute the script that trains the model and generates the final results:
    ```bash
    python SCRIPTS/02_analysis_and_model.py
    ```
    *This will save the model to `OUTPUT/final_model.pkl` and a summary of the results to `OUTPUT/results_summary.txt`.*

5.  **View Outputs:**
    All final reproducible figures and result files can be found in the **`OUTPUT/`** directory.

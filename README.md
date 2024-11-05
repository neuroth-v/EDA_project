[![Shipping files](https://github.com/neuefische/ds-eda-project-template/actions/workflows/workflow-03.yml/badge.svg?branch=main&event=workflow_dispatch)](https://github.com/neuefische/ds-eda-project-template/actions/workflows/workflow-03.yml)
# ds-project-template

Template for creating ds simple projects

## Project Overview

This repository provides a template for creating and organizing data science projects. It includes a basic project structure, essential dependencies, and guidance on setting up a virtual environment for development. The provided script (`housing_eda.py`) demonstrates a workflow for exploring a real estate dataset using various techniques. 

## Project Goals

This project aims to:

- **Clean and prepare the real estate dataset for analysis.** This includes handling missing values, correcting data types, and identifying and addressing outliers.
- **Explore the relationships between different features and the target variable (price).** This involves calculating correlations, performing statistical tests, and visualizing key findings.
- **Identify areas with the highest price premium for waterfront properties.** This helps understand the impact of location and waterfront status on pricing.
- **Analyze temporal patterns in property prices.** This reveals how prices fluctuate throughout the year based on seasonality and waterfront status.

## Repository Structure

The repository is structured as follows:

- **`EDA.ipynb`:** The main Python script containing the data analysis code. This script includes:
    - Data loading and initial data integrity checks.
    - Missing value imputation using various techniques.
    - Outlier detection and handling.
    - Feature engineering to create relevant new columns.
    - Statistical analysis to find correlations, perform ANOVA tests, and calculate effect sizes.
    - Visualizations using Matplotlib and Seaborn to highlight key findings.
    - A map visualization using Folium to display waterfront price premiums across different locations.
- **`data/`:** Directory for storing the real estate dataset file (i.e., `housing.csv`).
- **`GeoJSON/`:** Directory for storing the Seattle GeoJSON data used for the map visualization.
- **`requirements.txt`:** A file containing the list of dependencies required for the project.
- **`README.md`:** This file, providing an overview of the repository.

## Requirements

- **pyenv** for managing Python versions (optional but recommended)
- **python==3.11.3** the specific Python version used in the project
- **Node.js** required for using Plotly and Jupyter Lab

## Setup

**1. Set up Python Environment:**

* **Install pyenv (Optional):** If you don't have pyenv, follow the instructions at [https://github.com/pyenv/pyenv](https://github.com/pyenv/pyenv).
* **Install Python 3.11.3:**
    ```bash
    pyenv install 3.11.3
    pyenv local 3.11.3
    ```
* **Create a virtual environment:**
    ```bash
    python -m venv .venv
    ```
* **Activate the virtual environment:**
    ```bash
    source .venv/bin/activate  # macOS/Linux
    .venv\Scripts\Activate.ps1 # Windows PowerShell
    .venv\Scripts\activate     # Windows Git-Bash
    ```
* **Upgrade pip:**
    ```bash
    pip install --upgrade pip
    ```
* **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

**2. Install Node.js:**

- **Check Node version:**
    ```sh
    node -v
    ```
    If Node is not installed, follow the instructions below.
- **Install Node.js using Homebrew (macOS):**
    ```sh
    brew update
    brew install node
    ```
- **Install Node.js using Chocolatey (Windows):**
    ```sh
    choco upgrade chocolatey
    choco install nodejs
    ```

## Running the Script

1. Replace the placeholder `data/housing.csv` with your own real estate dataset. 
2. Run the script from your terminal:
    ```bash
    python EDA.ipynb
    ```

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for bug fixes, feature enhancements, or improvements to the analysis workflow.
   ```


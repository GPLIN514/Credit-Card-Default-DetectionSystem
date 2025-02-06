# Credit Card Default Detection System

This Shiny web application is designed to analyze and detect credit card defaults using various statistical techniques. The application includes functionalities such as data cleaning, variable selection, model training, and evaluation.

## 📂 Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Dataset](#dataset)
4. [Project Structure](#project-structure)
5. [Required Packages](#required-packages)
6. [Features](#features)
7. [Acknowledgments](#acknowledgments)

## 🛠 Installation
1. Ensure that you have R and RStudio installed.
2. Install the required packages by running the following command in R:
    ```R
    install.packages(c("shiny", "shinydashboard", "shinythemes", "plotly", "caret", "ggplot2", "pROC", "DT", "reshape2", "dplyr"))
    ```

## 📊 Dataset
Due to GitHub's file size limitations, the dataset is hosted on Google Drive.

🔗 **Download the dataset from Google Drive**:  
[Click here to download dataset.zip](https://drive.google.com/file/d/1ufkLRZVQ1yJs3Glfv0bBIwow-UxI6-Mv/view?usp=drive_link)

After downloading, extract the dataset and place it in the `data/` folder of this repository.

## 🚀 Usage
1. Set the working directory to the application location:
    ```R
    setwd("/home/user/documents/file")
    ```
2. Load the necessary R scripts:
    ```R
    source('bigdata/prog_clean.R')
    source('bigdata/var_type_select.R')
    source('bigdata/mutifo_fun.R')
    source('bigdata/feat_select.R')
    source('bigdata/test_clean.R')
    source('bigdata/pred_test_data.R')
    ```
3. Run the Shiny application:
    ```R
    runApp('app_final.R')
    ```

## 📁 Project Structure
- `app_final.R` - Main R script for the Shiny application.
- `bigdata/` - Directory containing R scripts for data processing and modeling.
  - `prog_clean.R` - Cleans the training dataset.
  - `var_type_select.R` - Selects numerical or categorical variables for sampling.
  - `mutifo_fun.R` - Analyzes categorical variables' impact on target variables.
  - `feat_select.R` - Analyzes numerical variables' impact on target variables.
  - `test_clean.R` - Cleans the test dataset.
  - `pred_test_data.R` - Generates models and predictions.
- `data/` - Directory where the extracted dataset should be placed.

## 📦 Required Packages
This application depends on the following R packages:
- shiny = 1.8.1.1
- shinydashboard = 0.7.2
- shinythemes = 1.2.0
- plotly = 4.10.4
- caret = 6.0-94
- ggplot2 = 3.5.0
- pROC = 1.18.5
- DT = 0.33
- reshape2 = 1.4.4
- dplyr = 1.1.4
- R version 4.3.3 (2024-02-29 ucrt)

## 🔥 Features
- **Home**: Overview of the application.
- **All Users**:
  - **Data Summary**: Summary statistics and visualizations of the dataset.
  - **Risk Analysis**: Analysis of factors leading to credit card defaults.
- **Individual Users**: Detailed analysis for specific users.

## 🙏 Acknowledgments
Special thanks to the professor of Big Data Analysis and my teammates for their contributions!


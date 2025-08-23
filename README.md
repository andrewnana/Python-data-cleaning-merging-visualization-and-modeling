# Background
In this notebook, we will analyze the 2022 PLACES (Population Level Analysis and Community Estimates) data from the CDC and the 2020 American Community Survey (ACS) data to explore social determinants of health and their relationship with chronic diseases. The analysis will focus on understanding how various social factors influence health outcomes in different communities. It will involve pulling the data from the ACS data from the Census API, cleaning, transforming and merging it with the PLACES dataset that was previously downloaded. Pulling the census data requires a key which is freely accessible after registration at https://api.census.gov/data/key_signup.html. We will perform exploratory data analysis (EDA) and visualization to gain insights into the data. We will later assess area-level associations between sdh and chronic illnesses. The data was analyzed using Python 313 on VS code.

Disclaimer: This analysis is intended for educational and research purposes only and has not been peer-reviewed. While efforts have been made to ensure the accuracy of the methods and results, the author does not guarantee the correctness or completeness of the analysis. The author bears no responsibility or liability for any errors, omissions, or outcomes resulting from the use of this material. Use at your own discretion

# Purpose
- Pull data from the ACS using a personal API key
- Upload the CDC PLACES 2022 dataset
- Merge the two datasets by ZCTAs
- Preprocess and clean the dataset
- Explore the dataset through data visualization
- Provide a summary statistic table based on chosen variables
- Proceed with statistical modeling

# Libraries used
- pandas
- numpy
- statsmodels
- seaborn
- matplotlib
- tableone # for summary statistics
- scipy.cluster
- missingno # for missing data visualization
- requests
- census
- us
- warnings
- collections # OrderedDict to maintain the order of columns

# Content

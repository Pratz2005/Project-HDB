Miniproject - HDB DATASET

In this project, we delve into analyzing HDB (Housing Development Board) sales data in Singapore and explore machine learning techniques to aid in predicting future finances for Singaporeans. With the rising cost of living and housing prices in Singapore, understanding and managing expenses when purchasing HDBs has become increasingly important.

## Problem Statement
Our central objective is to help Singaporeans predict their future finances more accurately. Given the continuous increase in HDB prices and the challenge of managing household expenses, we aim to develop models that provide insights into financial planning, especially concerning HDB purchases.

## Data Sources
- **Main Dataset**: Contains over 800,000 HDB sales records from 1990 to 2021. Each record includes information such as the size, type of flat, and geographic data.
- **RPI Table**: Resale Price Index data from 1990 to 2023, providing insights into housing market trends.
- **Household Expenditure Data**: Recorded 5-yearly Singapore Monthly household expenditure by flat type, offering insights into household spending patterns.

## Models Used
- **Linear Regression**: Initially used to predict financial aspects, but due to its limitations in capturing complex relationships, we transitioned to multivariate linear regression, achieving a decent R^2 of 0.8, but left many outliers and had a higher-than-expected mean square error.
- **Decision Trees Classifier**: Employed to classify household types based on features like home size, price, year of sale, and monthly expected household expenditure. Achieved 96% accuracy but dropped some information, such as the classification of "Multi-generational" flats.
- **Random Forest Classifier**: Utilized to refine the decision tree by generating multiple trees with randomness and averaging their decisions using regression. Achieved 98% accuracy with 10 trees of depth 4, using features like home size, household expenditure, and sale price.
- **Naive Bayes Classifier**: Applied to classify flat types based on expenditure and area square footage of the home. Achieved 96% accuracy, assuming a normalized distribution of the data.

## Libraries Used
- Pandas
- Seaborn
- NumPy
- Matplotlib
- mpl-tools
- scikit-learn
- SciPy

## File List
- `SC1015_MiniProject.ipynb`: Jupyter Notebook project file
- `ALL Prices 1990-2021 mar.csv`: Main dataset, more than 800,000 HDB sales records from 1990 to 2021 (Due to the large size of this file, we have split it into 5 zip files, kindly go through all)
- `RPI Table 2023_1990.xlsx`: Excel containing RPI Data from 2023 to 1990
- `Household expenditure_5yearly.xlsx`: Excel containing recorded 5 yearly Singapore Monthly household expenditure by flat type
- `AllPriceMetadata.txt`: Metadata information for ALL Prices 1990-2021 mar.csv

## Conclusion
Our project aims to provide Singaporeans with better financial planning tools, considering the challenges posed by rising HDB prices and living costs. Through machine learning techniques and data analysis, we strive to empower individuals to make informed decisions regarding their future finances.

## What Have We Learned?
- Linear regression, especially for complex response variables, may have limitations, but multivariate regression can provide more useful results.
- Random Forests offer a thorough approach to decision tree models, while classifiers like Decision Trees and Naive Bayes provide clearer responses and visualization.
- Monthly household expenditure is closely related to the type of home one lives in, rather than changes in the housing market. Additionally, expenditure per household tends to rise in relation to the rate of general inflation.

## Individual Contributions
- **Low Jun Keat**: Linear Regression, Classification, Random Forest, Presentation
- **Mehra Pratham**: Data Analysis and Cleaning, Naive Bayes, Presentation

## References
- [Kaggle - Singapore HDB Flat Resale Prices 1990-2020](https://www.kaggle.com/datasets/teyang/singapore-hdb-flat-resale-prices-19902020)
- [SingStat - Table Builder](https://tablebuilder.singstat.gov.sg/)
- [Smart Wealth - Cost of Living in Singapore Statistics](https://smartwealth.sg/cost-of-living-in-singapore-statistics/#:~:text=From%202014%2D2019%2C%20Singapore%20was,climbed%20up%20to%20second%20place)
- [Nimbus Homes - Rising Cost of Living in Singapore](https://www.nimbushomes.com/blog/rising-cost-of-living-in-singapore)
- [NUS ScholarBank - Research Paper](https://scholarbank.nus.edu.sg/handle/10635/220873#:~:text=The%20findings%20have%20shown%20that,net%20price%20decline%20of%204.62%25)


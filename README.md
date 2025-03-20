# Facebookads

## Overview
<p>This study explores the dynamics of political advertising on Facebook targeting Australian
audiences, using data from the Facebook Ad Library API for the period from October 1, 2023,
to March 21, 2024. This timeframe captures significant political events, including the
aftermath of the Voice referendum, providing a rich context for analyzing trends in political
communication. To further analysis, this proejct aim to investigate the relationship between
attributes and impressions.</p>

## Dataset description
The dataset under study comprises sponsored political ads from the Facebook Ad Library
API. This dataset covers a period from October 1, 2023, to March 21, 2024. The data is
structured in JSON format and contains detailed records of ad campaigns. The dataset
consists of 17475418 rows and 26 columns with diUerent types. These columns reflecting
various aspects of the ad campaigns, including content creation details (ad_creation_time),
creative details, campaign delivery metrics, and demographic targeting.

## How to Run the Project


### Prerequisites
#### **1. Required Software**
- **Python 3.x** ([Download Here](https://www.python.org/downloads/))
- **Apache Spark** (For distributed data processing)
- **Java 8 or later** (Required for Spark)
- **NLTK** (For natural language processing)
- **Matplotlib & Seaborn** (For data visualization)
- **NumPy & Pandas** (For numerical and data manipulation)
- **scikit-learn** (For machine learning models and preprocessing)
- **Gensim** (For topic modeling and word embeddings)

## Key Features
### Preprocessing
- Data cleaning: Null values removal and null values replacement
- Data transformation
- Text processing: Word tokens, URL cleaning, and TF-IDF
- Data exploration
- Feature correlation analysis
- Model prediction
- Model evaluation
- Feature importance
### Model used
- Random Forest

## Result
### EDA
<div align="center"><img width="500" alt="image" src="https://github.com/user-attachments/assets/b551de08-873a-4720-ae7e-0a06c725748f" />
</div>
<div align="center"><b>Figure 1: </b>Total Impressions by Page Name</div>

<div align="center"><img width="500" alt="image" src="https://github.com/user-attachments/assets/1a1d87b5-481d-4615-b80b-68d20687ac9d" />
</div>
<div align="center"><b>Figure 2: </b>Sum of Impressions by Gender and Age</div>

<div align="center"><img width="628" alt="image" src="https://github.com/user-attachments/assets/00e963e6-efd1-42d6-95cb-279eb2cc1e4e"/></div>
<div align="center"><b>Figure 3: </b>Top 20 TF-IDP Scores for Keywords in Ad Descriptions</div>

### Feature analysis
<div align="center"><img width="500" alt="image" src="https://github.com/user-attachments/assets/988b2436-7bdb-4e26-93ad-d7b1b7990b19"/>
</div>
<div align="center"><b>Figure 4: </b>Analysis of the Heatmap</div>

### Classification report
<table>
  <tr>
    <th></th>
    <th>Precision</th>
    <th>Recall</th>
    <th>F1-Score</th>
    <th>Support</th>
  </tr>
  <tr>
    <td>Over 50k</td>
    <td>1.00</td>
    <td>0.64</td>
    <td>0.78</td>
    <td>28</td>
  </tr>
  <tr>
    <td>Under 50k</td>
    <td>1.00</td>
    <td>1.00</td>
    <td>1.00</td>
    <td>8930</td>
  </tr>
  <tr>
    <td>Accuracy</td>
    <td></td>
    <td></td>
    <td>1.00</td>
    <td>8958</td>
  </tr>
  <tr>
    <td>Macro avg</td>
    <td>1.00</td>
    <td>0.82</td>
    <td>0.89</td>
    <td>8958</td>
  </tr>
  <tr>
    <td>Weighted avg</td>
    <td>1.00</td>
    <td>1.00</td>
    <td>1.00</td>
    <td>8958</td>
  </tr>
</table>

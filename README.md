# NY Housing Data Analysis

**Residency Project Day 1 — Group 1**  
**Course:** Python Application for Data Analytics in AI  
**Professor:** Najam Hassan  
**Team:** Sai Manasa Yadlapalli, Vineeth Avvaru, Ismail Oluwatobiloba Sule-Odu

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/manasayadlapalli/NY-Housing-Data-Analysis/blob/main/NY_Housing_Price_Prediction.ipynb)

## Project overview
A Python data analytics solution that predicts New York City home listing prices from property attributes (size, beds, baths, property type, borough, location). This deliverable covers **data preprocessing and initial model development**.

## Repository contents
| File | Description |
|---|---|
| `NY_Housing_Price_Prediction.ipynb` | Google Colab notebook: data exploration, cleaning, feature engineering, EDA charts and model training/evaluation |
| `NY_Housing_Project_Report.pdf` | Written report in APA 7 format (Introduction & Problem Framing, Dataset Exploration & Preprocessing, Initial Model Development, Team Collaboration) |
| `NY-House-Dataset.csv` | NY Housing Market dataset (4,801 listings, 17 columns), sourced from Kaggle |

## Key results (test set, 20% hold-out)
| Model | R² (log price) | MAE ($) | Median % error |
|---|---|---|---|
| Baseline (median) | -0.01 | 1,173,339 | 50.3% |
| Linear Regression | 0.73 | 746,692 | 27.8% |
| Random Forest | **0.89** | **497,878** | **18.3%** |
| Gradient Boosting | 0.86 | 544,924 | 20.4% |

Main data-quality findings: 214 duplicate rows, ~1/3 of square-footage values pre-filled with the column mean, a placeholder price of $2,147,483,647, and 21 inconsistent labels for NYC's 5 boroughs.

## How to run
1. Click **Open in Colab** above (or open the notebook locally with Jupyter).
2. Run the first code cell and upload `NY-House-Dataset.csv` when prompted (locally, keep the CSV next to the notebook).
3. Run all cells.

**Libraries:** pandas, NumPy, Matplotlib, Seaborn, scikit-learn

## Dataset
Elgiriyewithana, N. (2024). *New York housing market* [Data set]. Kaggle. https://www.kaggle.com/datasets/nelgiriyewithana/new-york-housing-market. Included here for reproducibility of a class project; all rights remain with the original dataset author.

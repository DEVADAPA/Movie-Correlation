# Movie Revenue Correlation Analysis

## Overview

This project analyzes a dataset of movies to identify the primary drivers of gross revenue. The analysis uses Python with Pandas for data manipulation, and Matplotlib/Seaborn for visualization. The core of the project is a Pearson correlation matrix used to quantify the relationship between different movie features (like budget, score, and votes) and their impact on gross earnings.

## Key Findings

From the correlation analysis, the two strongest drivers of gross revenue are:

* **Budget vs. Gross:** The strongest correlation found is between a film's `budget` and its `gross` revenue, with a Pearson coefficient of **~0.74**.
* **Votes vs. Gross:** Audience engagement (number of `votes`) is the second-strongest driver, correlating with `gross` revenue at **~0.63**.

The regression plot below visually confirms the strong positive trend between budget and gross revenue:

<img width="1042" height="731" alt="image" src="https://github.com/user-attachments/assets/4a3196e0-5340-47ef-aec5-edbdd092a162" />
<img width="1040" height="718" alt="image" src="https://github.com/user-attachments/assets/ed4fb9ad-1b9d-4f8d-8038-1f301815b070" />



## Project Process

1.  **Data Loading:** The `movies.csv` dataset was loaded into a Pandas DataFrame.
2.  **Data Cleaning:** Missing values were handled, and data types for `budget` and `gross` were converted to numeric types for analysis.
3.  **Data Transformation:** To create a comprehensive correlation matrix, all categorical (object) columns like `genre`, `rating`, and `company` were converted into numeric codes.
4.  **Visualization:**
    * A scatter plot and regression plot were created to visualize the relationship between `budget` and `gross`.
    * A full correlation heatmap was generated with Seaborn to show relationships between all numeric features at a glance.
5.  **Analysis:** The correlation matrix was unstacked and sorted to identify the highest positive and negative correlations.

## Technologies Used

* Python
* Pandas
* Numpy
* Seaborn
* Matplotlib
* Jupyter Notebook

## How to Run

1.  Clone this repository.
2.  Install the required libraries:
    `pip install -r requirements.txt`
3.  Open and run the `Movie Correlation Project.ipynb` notebook in Jupyter.

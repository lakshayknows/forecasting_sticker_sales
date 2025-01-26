# Sales Forecasting Dataset Analysis

This repository contains a Jupyter Notebook that analyzes and preprocesses a dataset for a sales forecasting problem. The dataset includes information about product sales across multiple countries, stores, and years. Below is a detailed description of the project and the steps performed.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Preprocessing Steps](#preprocessing-steps)
4. [Data Visualization](#data-visualization)
5. [How to Run](#how-to-run)
6. [Dependencies](#dependencies)
7. [Contributing](#contributing)
8. [License](#license)

---

## Project Overview

The objective of this project is to explore and preprocess a sales dataset to prepare it for machine learning modeling. The dataset contains information such as the date of sales, country, store, product type, and the number of units sold. Key tasks include handling missing values, feature engineering, and visualizing data distributions.

---

## Dataset Description

### Train Dataset:
- **Rows:** 230,130
- **Columns:** 6
  - `id`: Unique identifier
  - `date`: Date of the record
  - `country`: Country where the sales occurred
  - `store`: Store type
  - `product`: Product type
  - `num_sold`: Number of units sold (target variable)

### Test Dataset:
- **Rows:** 98,550
- **Columns:** 5
  - `id`: Unique identifier
  - `date`: Date of the record
  - `country`: Country where the sales occurred
  - `store`: Store type
  - `product`: Product type

---

## Preprocessing Steps

1. **Datetime Conversion:**
   - Converted the `date` column to `datetime` format.
   - Extracted `year`, `quarter`, and `month` as new features.

2. **Handling Missing Values:**
   - Identified 8,871 missing values in the `num_sold` column.
   - Planned strategies for imputation (e.g., KNN Imputer or statistical methods).

3. **Feature Engineering:**
   - Removed the `date` column after extracting time-based features.
   - Dropped the `id` column to avoid data leakage.

4. **Data Types Optimization:**
   - Optimized data types to reduce memory usage.

---

## Data Visualization

- **Categorical Variables:**
  - Visualized the distribution of categorical variables like `country`, `store`, and `product` using bar plots.
  - Annotated bar plots with count values for better interpretability.

- **Numerical Variables:**
  - Analyzed distributions of numerical variables such as `num_sold` using summary statistics and histograms.

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/sales-forecasting-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd sales-forecasting-analysis
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open the notebook file and execute the cells step by step.

---

## Dependencies

The following Python libraries are required:

- pandas
- numpy
- matplotlib
- seaborn

You can install these using the following command:
```bash
pip install pandas numpy matplotlib seaborn
```

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your enhancements. Ensure that your code follows the project’s coding standards.

---

## License

This project is licensed under the MIT License. See the LICENSE file for more details.


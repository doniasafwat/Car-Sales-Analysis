# Car Sales Data Science Project

A complete data science project focused on analyzing car sales data. It covers data cleaning, exploratory data analysis (EDA), web scraping from cars.com, data integration, visualization, and statistical hypothesis testing.

**Author:** Donia Safwat

---

## Project Structure

```
car-sales-ds/
├── data/
│   ├── raw/
│   │   └── car_data.csv                    # Original car sales dataset
│   └── processed/
│       ├── cleaned_data.csv                # Cleaned version of the original data
│       ├── scraped_data.csv                # Raw data scraped from cars.com
│       ├── cleaned_scraped_data.csv        # Cleaned and structured scraped data
│       ├── merged_data.csv                 # Combined original + scraped datasets
│       └── average_prices_by_dealer_and_model.csv
├── notebooks/
│   ├── 01_car_sales_analysis.ipynb         # Part 1: Cleaning, EDA & insights
│   └── 02_web_scraping_car_dealers.ipynb   # Part 2: Scraping, merging & hypothesis testing
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Tech Stack

| Category          | Libraries                                      |
|-------------------|------------------------------------------------|
| Data Handling     | pandas, numpy                                  |
| Visualization     | matplotlib, seaborn                            |
| Machine Learning  | scikit-learn                                   |
| Web Scraping      | BeautifulSoup4, requests                       |
| Statistics        | scipy                                          |
| Environment       | Jupyter Notebook                               |

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/car-sales-ds.git
cd car-sales-ds
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv

# Windows
venv\Scripts\activate

# macOS / Linux
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the notebooks

```bash
jupyter notebook
```

Run the notebooks in order:

1. `notebooks/01_car_sales_analysis.ipynb`
2. `notebooks/02_web_scraping_car_dealers.ipynb`

> **Note:** The second notebook performs live web scraping from cars.com. Results may vary over time depending on the website content and structure.

---

## Project Overview

### Part 1 – Car Sales Analysis
- Load and explore the original car sales dataset
- Handle missing values, duplicates, and outliers
- Perform exploratory data analysis (EDA)
- Analyze customer behavior by gender, region, income, and preferences
- Visualize body style preferences, seasonal trends, and dealer performance

### Part 2 – Web Scraping & Advanced Analysis
- Scrape live car listings from [cars.com](https://www.cars.com)
- Clean and transform the scraped data
- Merge scraped data with the original dataset
- Analyze relationships between:
  - Dealership ratings and car prices
  - Mileage and price
  - Dealership performance metrics
- Conduct hypothesis testing using Pearson correlation

---

## Key Insights

- Different regions show distinct preferences for car body styles (SUV and Hatchback dominate)
- Austin consistently leads in total sales volume
- Customer gender and annual income influence purchasing patterns
- Lower mileage vehicles tend to command higher prices
- Dealership ratings show varying relationships with pricing strategies


---

## Notes

- All file paths inside the notebooks are relative and work correctly when the notebooks are run from the `notebooks/` directory.
- The datasets are included for full reproducibility.
- The scraping notebook may require updates if the HTML structure of cars.com changes.

---

## License

This project is intended for educational purposes.

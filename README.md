# Instacart Grocery Basket Analysis

## Project Overview

This project analyzes customer shopping behavior using a modified Instacart dataset.  
The goal is to clean the data, handle missing and duplicated values, and perform exploratory data analysis (EDA) to identify purchasing patterns.

The analysis focuses on questions such as:

- When do customers usually place orders?
- Which days of the week have the highest order volume?
- How long do customers wait before placing another order?
- Which products are purchased most frequently?
- Which products are commonly reordered?
- What items are usually added first to the cart?

---

## Business Context

Instacart is a grocery delivery platform where customers place online grocery orders and receive them at home.

Understanding customer behavior can help businesses:

- Improve inventory planning
- Identify high-demand products
- Understand reorder behavior
- Optimize marketing strategies
- Improve customer experience

---

## Dataset

The project uses five datasets:

| File | Description |
|---|---|
| `instacart_orders.csv` | Information about customer orders |
| `products.csv` | Product information |
| `order_products.csv` | Products included in each order |
| `aisles.csv` | Aisle information |
| `departments.csv` | Department information |

---

## Tools Used

- Python
- pandas
- matplotlib
- Jupyter Notebook

---

## Project Steps

### 1. Data Overview

The first step was to load the datasets and inspect their structure, including:

- Number of rows and columns
- Data types
- Missing values
- General organization of the tables

### 2. Data Preprocessing

In this step, I prepared the data for analysis by:

- Checking and correcting data types
- Identifying duplicated records
- Removing duplicated orders
- Handling missing values
- Replacing unknown product names with `"Unknown"`
- Filling missing `add_to_cart_order` values with `999`

### 3. Exploratory Data Analysis

The analysis included:

- Order distribution by hour of the day
- Order distribution by day of the week
- Days since prior order
- Comparison between Wednesday and Saturday order times
- Distribution of number of orders per customer
- Top 20 most purchased products
- Most frequently reordered products
- Products most often added first to the cart

---

## Key Insights

- Most orders happen during the day, especially from morning to early afternoon.
- Sunday is one of the strongest days for grocery purchases.
- Bananas were the most purchased product in the dataset.
- Many customers repeatedly buy essential products.
- Missing values in `add_to_cart_order` were associated with large orders containing more than 64 products.

---

## Sample Results

### Top 10 Most Purchased Products

| Rank | Product | Orders |
|---|---|---:|
| 1 | Banana | 66,050 |
| 2 | Bag of Organic Bananas | 53,297 |
| 3 | Organic Strawberries | 37,039 |
| 4 | Organic Baby Spinach | 33,971 |
| 5 | Organic Hass Avocado | 29,773 |
| 6 | Organic Avocado | 24,689 |
| 7 | Large Lemon | 21,495 |
| 8 | Strawberries | 20,018 |
| 9 | Limes | 19,690 |
| 10 | Organic Whole Milk | 19,600 |

---

## Conclusion

This project showed how data cleaning and exploratory analysis can reveal important customer shopping patterns.

By analyzing Instacart order data, it was possible to identify peak shopping hours, popular products, reorder behavior, and customer purchasing habits.

The project also reinforced the importance of preprocessing data before drawing conclusions, since missing and duplicated values can affect the quality of the analysis.

---

## Repository Structure

```text
instacart-grocery-analysis/
│
├── data/
│   └── README.md
│
├── images/
│   └── README.md
│
├── notebooks/
│   └── instacart_analysis.ipynb
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## Author

**André Luiz de Azevedo Monte**  
Sales Manager transitioning into Data Analytics  
Mexico City | Open to remote opportunities

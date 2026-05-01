# UrbanStyle Customer Data Cleaning

## Module 10 Assignment: Data Manipulation and Cleaning with Pandas

A Python data cleaning and preprocessing project focused on customer transaction data for **UrbanStyle**, a retail fashion company. This project demonstrates practical use of **Pandas** for cleaning messy datasets, correcting inconsistencies, engineering useful features, and generating business insights from customer purchase behavior.

---

## Project Overview

This project simulates a real-world retail customer dataset containing common data quality issues such as:

- Missing values
- Duplicate records
- Inconsistent date formats
- Currency formatting inconsistencies
- Mixed text capitalization
- Phone number formatting issues

The script cleans and standardizes the dataset to create an analysis-ready DataFrame for business intelligence reporting.

---

## Objectives

The project performs the following tasks:

### 1. Load and Explore Data
- Load customer data from a simulated CSV file
- Inspect dataset structure
- Identify missing values
- Detect duplicate records

### 2. Handle Missing Values
- Fill missing satisfaction ratings using median values
- Forward-fill missing purchase dates
- Replace missing:
  - Last names
  - Phone numbers
  - Loyalty status
  - Age values

### 3. Correct Data Types
- Convert date columns to datetime format
- Convert currency-formatted text to numeric values
- Ensure numeric consistency across fields

### 4. Standardize Text Data
- Convert names to proper case
- Normalize category naming conventions
- Standardize phone numbers to:

```text
XXX-XXX-XXXX
```

### 5. Remove Duplicate Records
- Detect duplicated customers
- Retain unique entries

### 6. Feature Engineering
Create derived analytical features:

- **Days Since Last Purchase**
- **Average Purchase Value**
- **Purchase Frequency Category**
  - High
  - Medium
  - Low

### 7. DataFrame Cleanup
- Rename columns for readability
- Remove unnecessary columns
- Sort by revenue contribution

### 8. Generate Business Insights
Analyze:

- Average spending by loyalty status
- Revenue by product category
- Correlation between satisfaction and spending

### 9. Final Reporting
Generate a complete data quality and business insights report.

---

## Technologies Used

- **Python 3**
- **Pandas**
- **NumPy**
- **Datetime**

---

## Project Structure

```text
urbanstyle-customer-cleaning/
│
├── urbanstyle_cleaning.py
├── README.md
```

---

## Dataset Fields

The simulated dataset contains:

| Column | Description |
|-------|------------|
| customer_id | Unique customer identifier |
| first_name | Customer first name |
| last_name | Customer last name |
| email | Customer email |
| phone | Contact number |
| join_date | Membership start date |
| last_purchase | Most recent purchase |
| total_purchases | Number of purchases |
| total_spent | Total customer spending |
| preferred_category | Favorite shopping category |
| satisfaction_rating | Customer satisfaction score |
| age | Customer age |
| city | Customer city |
| state | Customer state |
| loyalty_status | Loyalty program level |

---

## Key Data Cleaning Techniques Demonstrated

### Missing Value Imputation
Uses:
- Median substitution
- Forward fill
- Default placeholder values

### String Cleaning
Uses:
- `.str.title()`
- `.str.strip()`

### Regex Replacement
Used to remove:

- Dollar signs (`$`)
- Commas (`,`)

from currency values.

### Phone Formatting
Custom function standardizes all phone entries.

---

## Business Insights Generated

The script identifies:

### Customer Metrics
- Total customer count
- Purchase frequency segmentation

### Revenue Analysis
- Average spending by loyalty tier
- Highest-performing product categories

### Customer Behavior
- Spending patterns
- Satisfaction vs. spending correlation

---

## Example Output

```text
URBANSTYLE CUSTOMER DATA CLEANING REPORT

Data Quality Issues:
- Missing Values: X total missing entries
- Duplicates: X duplicate records found

Standardization Changes:
- Names converted to proper case
- Categories standardized
- Phone numbers reformatted

Key Business Insights:
- Customer Base: X total customers
- Top Category: Womenswear
- Revenue by Loyalty Status
```

---

## Learning Outcomes

This project demonstrates proficiency in:

- Data cleaning with Pandas
- Data preprocessing
- Feature engineering
- Exploratory data analysis
- Business reporting automation

---

## How to Run

### Clone the Repository

```bash
git clone https://github.com/your-username/urbanstyle-customer-cleaning.git
cd urbanstyle-customer-cleaning
```

### Install Dependencies

```bash
pip install pandas numpy
```

### Run the Script

```bash
python urbanstyle_cleaning.py
```

---

## Author

**Ziyuan Zhang**

Module 10 Assignment  
Data Manipulation and Cleaning with Pandas

---

## License

This project is for academic and educational purposes.

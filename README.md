# 🛒 Supermarket Sales Analysis & EDA

## 📖 Project Overview

This repository provides an end-to-end **Exploratory Data Analysis (EDA)** on retail supermarket sales data across three separate branches (**Yangon**, **Mandalay**, and **Naypyitaw**) over a 3-month period.

The primary objective is to analyze customer purchasing behavior, revenue distribution across product lines, transaction channels, and branch performances to extract actionable retail business intelligence.

---

## 📊 Dataset Architecture

The analysis is performed on historical transaction records comprising **1,000 observations** and **17 features** with **zero missing values** and **zero duplicate records**.

### Data Dictionary

| Column Name | Type | Description |
| :--- | :---: | :--- |
| `Invoice ID` | String | Unique identifier generated for each invoice transaction |
| `Branch` | Categorical | Branch code identifier (`A`, `B`, `C`) |
| `City` | Categorical | City location of the branch (`Yangon`, `Mandalay`, `Naypyitaw`) |
| `Customer type` | Categorical | Membership category (`Member`, `Normal`) |
| `Gender` | Categorical | Gender of the customer (`Male`, `Female`) |
| `Product line` | Categorical | Item category (e.g., Food & beverages, Electronic accessories, Fashion accessories) |
| `Unit price` | Float | Price per item in USD |
| `Quantity` | Integer | Number of items purchased per transaction |
| `Tax 5%` | Float | 5% value-added tax applied to the purchase |
| `Total` | Float | Total transaction cost including tax |
| `Date` | Date | Date of transaction recorded |
| `Time` | Time | Timestamp of purchase |
| `Payment` | Categorical | Payment method used (`Ewallet`, `Cash`, `Credit card`) |
| `cogs` | Float | Cost of Goods Sold |
| `gross margin percentage` | Float | Fixed profit margin percentage (4.76%) |
| `gross income` | Float | Net gross income generated |
| `Rating` | Float | Customer satisfaction rating (scale: 1.0 to 10.0) |

---

## 💡 Key Business Insights

- **Branch Performance Parity:** Sales revenue is uniformly distributed across the three branches, with Branch C marginally leading in total transaction value.
- **Leading Categories:** `Food and beverages`, `Fashion accessories`, and `Electronic accessories` represent the primary revenue drivers.
- **Payment Distribution:** Adoption of digital payments (`Ewallet`), physical `Cash`, and `Credit card` is remarkably balanced (~33-34% each), indicating frictionless checkout options for consumers.
- **Demographic Balance:** Purchase volume and gross revenue show equitable distribution across gender types and membership tiers (`Member` vs. `Normal`), highlighting broad-spectrum market appeal.

---

## 📈 Visualizations & Analysis

The Jupyter Notebook (`supermarket_sales_analysis.ipynb`) includes dedicated visual analyses:
- **Revenue by Branch:** Comparative bar plots illustrating aggregate revenue performance.
- **Product Line Contribution:** Categorical ranking of product categories by total sales.
- **Payment Method Preference:** Frequency distribution of customer payment channels.

---

## 📁 Repository Structure

```text
supermarket-sales-analysis/
│
├── supermarket_Sales.csv           # Cleaned transaction dataset
├── supermarket_sales_analysis.ipynb# EDA & data visualizations notebook
├── requirements.txt                # Required Python packages
├── README.md                       # Comprehensive documentation

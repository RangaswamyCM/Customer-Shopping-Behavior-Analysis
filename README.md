# 🛍️ Customer Shopping Behavior Analysis

## 📖 Overview
This project analyzes **customer shopping behavior** using real-world transactional data.  
The goal is to uncover insights into spending patterns, customer demographics, product preferences, and subscription trends to support **data-driven business decisions**.

The complete workflow covers:
- Data loading and preprocessing in Python  
- Exploratory Data Analysis (EDA)  
- SQL-based business analytics  
- Interactive Power BI dashboard creation  
- Final presentation and reporting using Gamma  

---

## 📊 Dataset
**Name:** Customer Shopping Behavior Dataset  
**Size:** 3,900 rows × 18 columns  

**Key Features:**
- Customer Demographics: `Age`, `Gender`, `Location`, `Subscription Status`  
- Purchase Details: `Item Purchased`, `Category`, `Purchase Amount`, `Season`, `Size`, `Color`  
- Behavioral Data: `Discount Applied`, `Promo Code Used`, `Previous Purchases`, `Review Rating`, `Shipping Type`  

**Missing Data:** 37 null values in `Review Rating` column (handled via median imputation per product category).

---

## 🧰 Tools & Technologies
| Category | Tools Used |
|-----------|-------------|
| Programming | Python (Pandas, NumPy, Matplotlib, Seaborn) |
| Database | PostgreSQL / MySQL / SQL Server |
| Dashboarding | Power BI |
| Presentation | Gamma |
| Environment | Jupyter Notebook / VS Code |

---

## ⚙️ Steps Followed

### 1. **Data Loading & Cleaning (Python)**
- Imported dataset using `pandas`.
- Handled missing values in `Review Rating` with category-wise median.
- Standardized column names to `snake_case`.
- Performed feature engineering:
  - Created `age_group` from `Age`.
  - Derived `purchase_frequency_days` from purchase timestamps.
- Removed redundant features (`promo_code_used`).

### 2. **Exploratory Data Analysis**
- Generated descriptive statistics using `.info()` and `.describe()`.
- Visualized:
  - Distribution of purchase amounts by category and gender.
  - Correlation between discounts and spending.
  - Subscription vs. revenue contribution.

### 3. **SQL Analysis**
Conducted key business analyses using SQL queries in PostgreSQL:
- Revenue comparison by gender.  
- High-spending discount users.  
- Top 5 products by average rating.  
- Shipping type vs. purchase amount.  
- Subscribers vs. non-subscribers.  
- Discount-dependent products.  
- Customer segmentation (New, Returning, Loyal).  
- Revenue by age group.

### 4. **Dashboard in Power BI**
Built an **interactive Power BI dashboard** to visualize:
- Revenue trends by gender, age group, and location.  
- Customer segment performance.  
- Product-wise sales and ratings.  
- Discount and subscription patterns.

### 5. **Final Report & Presentation**
- Created a concise **business report** summarizing key insights and recommendations.  
- Designed an engaging **Gamma presentation** for storytelling and stakeholder communication.  

---

## 📈 Results & Insights
- **Subscribers** contribute significantly higher revenue.  
- **Loyal customers** have stronger engagement and purchase frequency.  
- **Express shipping users** tend to spend more per purchase.  
- **Top-rated products** align with the highest-selling categories.  

**Recommendations:**
- Promote loyalty programs.  
- Refine discount strategies.  
- Target top-performing age and location segments.  


 📉 Layoffs EDA Using SQL

This project focuses on performing **Exploratory Data Analysis (EDA)** using SQL on a real-world dataset of global layoffs. The objective is to uncover trends, patterns, and business insights related to layoffs across various industries and companies.

---

## 🎯 Objective

Analyze the layoff dataset using SQL to understand:
- Which companies and industries had the most layoffs
- Year-wise and country-wise trends
- The impact of COVID-19 on layoffs
- Correlation between company size and layoffs

---

## 📁 Dataset

- **Name**: `layoffs.csv`
- **Source**: [layoffs.csv](https://drive.google.com/file/d/145S2GXv-3fv9boVABFNgLUMfh4y-3xXJ/view?usp=sharing)
- **Columns Include**:
  - `company`, `industry`, `total_laid_off`, `percentage_laid_off`
  - `location`, `country`, `date`, `stage`, `funds_raised`

---

## 🛠️ Tools Used

- **MySQL** for SQL queries
 **Drive** for video demo

---

## 🔍 Key Insights

- Top 10 companies with the highest layoffs
-  Industry-wise layoff distribution
-  Country and year-wise trends
-  Startups vs Funded companies layoffs comparison

---

## 📺 Demo Video

▶️ [Watch Demo Here](https://drive.google.com/file/d/1492BOFoUE4dfI07CESJKtO0ke3b7bd7J/view?usp=drive_link)

---

## 💻 Sample SQL Queries[layoffs.csv](https://github.com/user-attachments/files/21455222/layoffs.csv)


```sql
-- Total layoffs by industry
SELECT industry, SUM(total_laid_off) AS layoffs
FROM layoffs
GROUP BY industry
ORDER BY layoffs DESC;

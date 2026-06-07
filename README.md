# 🛒 Superstore Sales Performance Dashboard

An interactive Power BI dashboard analyzing 4 years of Superstore sales data (2011–2014), built to uncover revenue trends, customer behavior, product performance, and the impact of discounting on profitability.

---

## 📊 Dashboard Pages

| Page | Description |
|------|-------------|
| Overview | KPI cards (Total Sales, Profit, Orders), Sales by Category & Sub-Category Treemap, Year slicer |
| Geographic Analysis | Top 10 States for Technology Sales, Top 5 States for Office Supplies, Region slicer |
| Products Performance | Sub-Category Sales vs Profit — identifying winners and losers |
| Customer Analysis | Top 20 Customers ranked by Sales with profitability breakdown |
| Discount & Time Analysis | Discount impact on profit, Monthly sales trend, Busiest days of the week |
| Forecasting & Extras | 12-month sales forecast with 95% confidence interval, Discount vs Profit scatter plot |

---

## 🔍 Key Insights

- **California dominates** both Technology ($133K) and Office Supplies ($159K) — the store's most strategic market
- **Discounts are hurting the business** — discounted orders generated a net loss of -$160K while non-discounted orders made $440K profit
- **Tables is the biggest loss-maker** — $199K in sales but -$16K in profit due to heavy discounting
- **Copiers are the star performer** — highest profit-to-sales ratio across all subcategories
- **Sean Miller**, the top customer by sales ($25K), is actually generating a net loss of -$1,980
- **Friday is the busiest day** — weekday sales dominate, suggesting a B2B customer base
- **November & December peak** — best months for sales, worst time for discounts
- **Sales forecast** projects continued upward trend into 2015 with seasonal patterns maintained

---

## 🛠️ Tools & Skills Used

- **Power BI Desktop** — dashboard design and visualization
- **Power Query** — data cleaning, transformation, and relationship building
- **DAX** — calculated columns and measures
- **Data Modeling** — Star Schema with Orders (fact table), Products and CRM (dimension tables)

---

## 🧹 Data Issues Identified & Resolved

| Issue | Type | Resolution |
|-------|------|------------|
| Product ID format mismatch between Orders and Products tables | Structure | Extracted numeric portion to create matching key |
| 267 duplicate Product Short IDs in Products table | Data Quality | Removed duplicates keeping first occurrence |
| Misspelled column name "Orginal Price" | Data Quality | Renamed to "Original Price" in Power Query |
| Significant portion of orders with negative profit | Business Alert | Added "Profit Status" conditional column for visibility |

---

## 📁 Dataset

The dataset contains 3 related tables:
- **Orders** — 9,994 transactional records (2011–2014)
- **CRM** — 793 customer records
- **Products** — 1,862 product records

---

## 👩‍💻 Author

**Yomna Salama** — Data Science Graduate  
🔗 [LinkedIn](https://www.linkedin.com/in/yomna-salama-49799b31b/)  
🌐 [Portfolio](https://yomnasalama11.wixsite.com/yomnasalama)  
💻 [GitHub](https://github.com/yomnaSalamaa)

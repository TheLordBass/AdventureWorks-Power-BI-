# 🚴 AdventureWorks Cycles — Sales & Customer Dashboard (Power BI)

### 🚀 Executive Summary
**Goal:** Turn AdventureWorks Cycles' transactional data into a three-page Power BI report covering executive performance, customer profiling, and product-level profitability with what-if pricing.
**Role:** BI Developer.
**Tools:** Power BI Desktop (star-schema model, DAX measures, what-if parameters, drill-through navigation, date slicers).

---

## 📖 The Story
AdventureWorks sells bikes, clothing and accessories across Europe, North America and the Pacific. The commercial team needed more than a revenue total — they needed to know *who* is buying, *what* is carrying the profit, and *what happens to margin if we change price*.

The report is built in three layers: a summary that answers "how are we doing", a customer page that answers "who are they", and a product page that answers "what if we moved the price".

---

## 📊 The Dashboard

### 1. Executive Summary
![Executive summary page](Adventure%20Works%20exec%20summary.png)

Headline revenue, monthly orders and monthly returns against goal, with category and sub-category order breakdowns, a full product table showing orders and return rate side by side, and a geographic view of order distribution. Date range slider covers Jan 2016 – Jun 2017.

**What it shows:** $1.83M total revenue, running 3.31% ahead of the £1.77M goal, on 22,534 orders at a 2.14% blended return rate. The split that matters: **Water Bottle – 30 oz.** is the top product by *orders* while **Mountain-200 Black, 46** is top by *profit* — volume and value live in completely different parts of the catalogue. Tires and tubes lead sub-category volume at 9.1K orders.

### 2. Customer Detail
![Customer detail page](Adventure%20works%20Customer%20Detail.png)

Customer profiling by occupation, gender, income level and age, with a ranked table of top customers by revenue and a combined orders/revenue trend by month.

**What it shows:** 353 orders and $751,130 revenue from the profiled base, led by Maurice Shan (6 orders, $12.4K). Orders and revenue both step up sharply from Jul 2016 and hold — the growth is a level shift, not a seasonal bump. The occupation and income donuts show the base is concentrated in professional and skilled-manual segments rather than spread evenly.

### 3. Product Detail
![Product detail page](Adventure%20works%20Product%20Detail.png)

Single-product drill-through — orders, revenue and returns against target on gauges, weekly profit with a trend line and forecast band, weekly return volume, and a **what-if price adjustment slider** that recalculates adjusted profit live.

**What it shows:** For AWC Logo Cap, 232 orders and $4.03K revenue, both ahead of target, with 6 returns against a threshold of 5. The price slider at +50% lifts the average retail price from $8.64 to $12.96 and visibly separates adjusted profit from actual — the point of the page is letting a commercial manager test a pricing decision without waiting on an analyst.

---

## 🛠️ Technical Skills Demonstrated
* **Data modelling:** Star schema across sales, returns, products, customers, territories and calendar, with a dedicated date table for time intelligence.
* **DAX:** Goal-versus-actual measures, return rate, adjusted profit driven by a what-if parameter, weekly and monthly aggregations.
* **What-if parameters:** A price-adjustment slider that flows through to profit, turning a static report into a decision tool.
* **Drill-through navigation:** Executive summary → product detail with back-navigation, so one report serves both a 30-second read and a deep dive.
* **Visual selection:** Gauges for single-target tracking, trend lines with forecast bands for direction, treemaps for category share, conditional formatting to surface high return rates.

---

## 🗂️ Repository Contents

| File | What it is |
|---|---|
| `Adventureworks_Report.pbix` | The Power BI report — open in Power BI Desktop |
| `Adventure Works exec summary.png` | Page 1 screenshot |
| `Adventure works Customer Detail.png` | Page 2 screenshot |
| `Adventure works Product Detail.png` | Page 3 screenshot |

---

## 📊 Future Improvements
* **Returns analysis page:** Return rate varies from 0.68% to 3.75% across products with no explanation surfaced — a page linking returns to category, region and season would close that gap.
* **Currency consistency:** Revenue displays in dollars while goals display in pounds. Standardise on one.
* **Customer lifetime value:** The customer page ranks by revenue to date; a cohort-based CLV measure would make it forward-looking.

---

### 👋 About Me
Data Analyst based in **Manchester, UK**, working in **SQL, Excel, Tableau and Power BI**.
[LinkedIn](https://www.linkedin.com/in/ibomeno-basiekanem/) · [Portfolio](https://thelordbass.github.io/)

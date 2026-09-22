<div align="center">

# 📦 Amazon Sales Intelligence Dashboard
## *Regional, Product & Return Performance — Amazon India Marketplace*

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=E8720C&center=true&vCenter=true&width=750&lines=120.30K+Overall+Sales+%7C+19.25K+Sellers;Kaggle+Dataset+%E2%86%92+Power+BI+%E2%86%92+Interactive+Dashboard;Where+Are+We+Winning%2C+and+Where+Are+We+Losing%3F;Custom+Tooltip-on-Hover+Product+Drilldown" alt="Typing SVG" />

<br><br>

<img src="https://img.shields.io/badge/Power%20BI-3%20Page%20Dashboard-F2C811?logo=powerbi&logoColor=black"> <img src="https://img.shields.io/badge/Kaggle-Amazon%20Sale%20Report-20BEFF?logo=kaggle&logoColor=white"> <img src="https://img.shields.io/badge/Feature-Custom%20Tooltip%20Page-8A2BE2"> <img src="https://img.shields.io/badge/Status-Complete-success"> <img src="https://komarev.com/ghpvc/?username=Bernad2304&label=Repo%20Views&color=blueviolet&style=flat">

</div>

<br>

<div align="center">

## 🗺️ Table of Contents

| | | |
|:---:|:---:|:---:|
| 🎯 [Business Objective](#-business-objective) | 📁 [Dataset](#-dataset) | 🖥️ [Dashboard Structure](#️-dashboard-structure) |
| ❓ [Business Questions & Answers](#-business-questions--answers) | 📸 [Visual Gallery](#-visual-gallery) | 🧠 [Skills Applied](#-skills-applied) |
| 🚀 [About Me](#-about-me) | | |

</div>

---

## 🎯 Business Objective

An e-commerce seller sitting on order-level data can't just ask "how are we doing?" — that question is too broad to act on. This dashboard breaks it into something a business can actually use:

> **Which regions, cities, and individual products are driving real sales performance, and where is hidden cost — like returns — quietly eating into that performance?**

Built entirely from a public Kaggle dataset, styled after Amazon's own storefront UI so a non-technical stakeholder recognizes the interface instantly instead of learning a new one.

---

## 📁 Dataset

Sourced from Kaggle's **Amazon Sale Report** dataset — real Amazon India order-level data covering the April–June 2022 window, including order status, ship-to state/city, sales amount, units, and return/review figures. This was a self-directed project built on a public dataset, separate from client or employer data, to practice designing a dashboard around genuine e-commerce business questions rather than a guided tutorial.

---

## 🖥️ Dashboard Structure

The dashboard is built as three linked pages, styled to mirror Amazon's own navigation so it feels native to anyone who's ever shopped on the platform:

### 🏠 Overview
The landing page — overall sales, filtered sales, and seller count as headline KPIs, with **Sales by State**, **Sales by City**, and a **Sales by Year** trend line beneath. Includes a live **Status filter** (Cancelled, Pending, Shipped, Shipped–Damaged, Shipped–Lost in Transit, and more), so a viewer can isolate healthy completed sales from orders still at risk, instead of one blended number that hides the problem.

### 🛍️ Products
A visual product catalog page — each product shown with its image, name, and short description, letting a stakeholder browse the actual catalog rather than a table of SKU codes. This page exists to make the dashboard feel like a real merchandising tool, not just a numbers screen.

### 🔍 Product View
A drill-down page for a single selected product — Sale Amount, Units, Return(loss), and Review count as KPI cards, with a dedicated Units-by-Year trend chart and a date-range filter, so performance for any one product can be inspected in isolation instead of buried inside the aggregate.

### 💬 Custom Hover Tooltip — the feature I specifically built to learn
Rather than relying on Power BI's default hover tooltip (which just shows a single value), I designed a **custom tooltip page**: hovering over a product surfaces a full mini report card — Sale Amount, Units, Return(loss), Review, and its own Units-by-Year trend chart — right where the viewer's cursor already is. This means comparing two products no longer requires clicking away from the page they're on; the deeper numbers come to them instead. This was a deliberate choice to go past Power BI's default tooltip behavior and build a genuinely custom one from scratch.

---

## ❓ Business Questions & Answers

**Q: Which states are generating the most sales?**
Maharashtra leads at 21K, well ahead of Karnataka (16K), with Tamil Nadu and Telangana tied at 11K each. The gap between #1 and #2 (21K vs 16K) shows sales aren't evenly spread — they're concentrated.

**Q: Which cities matter most, and does city size predict sales?**
Not directly. Bengaluru tops the city list at 11.4K, ahead of even larger metros like Mumbai (6.8K) — meaning raw city population isn't the driver, something more specific to Bengaluru's market is.

**Q: How should "total sales" be interpreted, given real-world order problems?**
Carefully — the Status filter (Cancelled, Pending, Shipped–Damaged, Shipped–Lost in Transit, etc.) exists precisely so a stakeholder doesn't mistake a gross order count for confirmed, healthy revenue. An order marked "Shipped – Lost in Transit" shouldn't be counted the same as one marked "Shipped – Delivered to Buyer."

**Q: Did sales grow steadily over the quarter, or is there a pattern?**
Neither steady growth nor decline — the Apr–Jun 2022 trend oscillates in a repeating sawtooth pattern between roughly 1K and 2K, with a peak around mid-May. That's a cyclical demand pattern, not a simple trend line, and it matters because a business reading this as "flat growth" would miss the cyclicality entirely.

**Q: For an individual product, how significant are returns relative to sales?**
For the girls' t-shirt product drilled into, Return(loss) sits at 1.62M against a Sale Amount of 89.08M — roughly 1.8% of sales value lost to returns for that one item. Surfacing this per-product (not just as a company-wide average) is what lets a business catch a specific problem product instead of it hiding inside a healthy overall number.

---

## 📸 Visual Gallery

### Overview
Sales by state, sales by city, the live Status filter, and the quarterly sales trend — the landing page for the whole dashboard.
<p align="center"><img src="./Images/Overview.png" width="800"></p>

### Products
A browsable, image-based product catalog styled after Amazon's own storefront.
<p align="center"><img src="./Images/Products.png" width="800"></p>

### Product View
Single-product drill-down: Sale Amount, Units, Return(loss), Review, and a dedicated Units-by-Year trend for one selected item.
<p align="center"><img src="./Images/Product_View.png" width="800"></p>

### Custom Hover Tooltip
The feature built specifically to go beyond Power BI's default tooltip — a full mini report card appears on hover, right at the viewer's cursor.
<p align="center"><img src="./Images/Custom_Tooltip.png" width="800"></p>

---

## 🧠 Skills Applied

- **Custom Tooltip Design** — built a full report-page tooltip from scratch instead of relying on Power BI's default single-value hover, so comparative data appears exactly where the viewer's attention already is
- **UI/UX Replication** — styled the dashboard to mirror Amazon's own navigation and layout, making it immediately familiar to a non-technical stakeholder
- **Regional & Return Analysis** — broke down performance by state, city, and individual product, and specifically isolated return value against sales at the product level rather than only reporting an aggregate
- **Status-Aware Reporting** — built filtering around real order-status complexity (cancelled, lost in transit, damaged) instead of treating every order as a clean, completed sale

---

## 🚀 About Me

**Bernad Meckenzi S** — transitioning into Data Analytics / Business Intelligence. B.Sc. Mathematics, Loyola College, Chennai.

| 🔧 Skill Area | 🌟 Tools |
|---|---|
| 🗄️ Business Intelligence | Power BI, DAX, Power Query |
| 🐍 Programming | Python, Pandas, NumPy |
| 🗃️ Data Querying | SQL |
| ⚙️ Automation | n8n |

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-Bernad2304-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Bernad2304)

⭐ **If this helped you see how a dashboard turns raw order data into real business questions, a star would mean a lot.**

</div>

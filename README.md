# 📊 Inventory Funding & Supplier Analytics Dashboard (Power BI)

## Project Overview

An end-to-end, interactive **2-Page Power BI Dashboard** built for an **Inventory Funding System (IFS)**. This analytics solution integrates data across Sales & Revenue Performance, Banking Credit & Funding Gap Analysis, and Supply Chain Operations / Supplier Risk Management.

It provides business leaders and operations managers with a **360-degree view** to optimize funding allocation, mitigate supplier liability risks, and ensure streamlined inventory reorder management.

---

## 📸 Dashboard Screenshots & Design Layout

The dashboard is structured into two distinct views catering to Executive Decision-Making and Operational Risk Management.

### 📄 Page 1: Executive Overview (Financial & Sales Performance)
<img width="964" height="549" alt="inventory   funding analytics dashboard page1" src="https://github.com/user-attachments/assets/4cc39c24-6d0b-4531-9218-71c362cf8c14" />


### 📄 Page 2: Operational Stock & Supplier Analytics
<img width="965" height="546" alt="stock management   supplier analytics dashboard page2" src="https://github.com/user-attachments/assets/28aa1d6e-667e-4104-ba2f-e162c380fdba" />


---

## 💡 Key Features & Business Insights

### 📊 Page 1: Executive Overview
* **8 Core KPI Cards:** Real-time tracking of Total Order Value (₹129.85M), Total Revenue (₹179M), Total Profit (₹49.38M), Profit Margin % (27.55%), Total Funding Required vs. Approved, Funding Gap (₹21.08M), and Total Overdue Amount (₹4.94M).
* **Monthly Funding Trend:** Clustered Column Chart analyzing the monthly volume of Order Value vs. Approved Funding, highlighting liquidity trends.
* **Category Breakdown:** Granular analysis of sales performance and funding approval rates across product categories (Electronics, Furniture, Accessories, Stationery).
* **Funding Sources (Treemap):** Dynamic breakdown of total approved funding across various streams: Overdraft, Business Cash, Supplier Credit, and Working Capital Loans.
* **Payment Status Distribution:** Donut chart mapping total transaction volume (300 Counts) across defined statuses: Paid, Pending, Partially Paid, and Overdue.

### 📈 Page 2: Operational Risk Management
* **Reorder Alert Analysis:** Interactive dual-bar chart mapping product-level current stock against critical reorder limits to avoid stockouts.
* **Supplier Liability & Outstanding Debt:** Bar chart identifying top suppliers with the highest outstanding liabilities (e.g., Metro Wholesale - ₹11.2M, Prime Distributors - ₹9.5M).
* **Payment Terms Breakdown:** Segmentation of total outstanding liabilities by defined credit terms (Net 15, Net 30, Net 45, Advance) to manage cash flow risk.
* **Warehouse Distribution (Dual Axis Chart):** Professional Line and Clustered Column visual mapping regional inventory volume (Units) against total monetary value (₹ Millions) across strategic hubs (Nagpur, Nashik, Mumbai, Pune Central).

---

## 🛠️ Tech Stack & DAX Measures Used

* **BI Tool:** Microsoft Power BI Desktop
* **Data Modeling:** Star Schema / Relational Model
* **Key Custom DAX Formulas Included:**
  ```dax
  // Profit Margin Calculation
  Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)

  // Net Funding Shortfall
  Funding Gap = [Total Funding Required] - [Total Funding Approved]

  // Count of Items requiring Immediate Reorder
  Low Stock Count = CALCULATE(COUNTROWS('IFS_Data'), 'IFS_Data'[Current_Stock] <= 'IFS_Data'[Reorder_Level])

---

## 📂 Project Directory Structure
├── datasets/  
│    └── Inventory_funding_system_Dataset.csv  
├── images/  
│    ├── inventory & funding analytics dashboard page1.png  
│    └── stock management& supplier analytics dashboard page 2.png  
├── IFS_Dashboard_Project.pbix  
└── README.md  

---

## 🚀 How to view the project
1. Download the IFS_Dashboard_Project.pbix file from this repository.
2. Open it using Power BI Desktop.
3. Interact with the top slicer bar to filter data across Date, Region, Category, Inventory Item, Payment Status, Supplier, or Warehouse.

---

## 👤 Author & Contact

* **Developer:** Niranjan Rathod
* **Role:** Data Analyst / Power BI Developer
* **GitHub:** [[your-github-username](https://github.com/your-github-username)](https://github.com/Niranjan613/INVENTORY-FUNDING-ANALYTICS-DASHBOARD/new/main?filename=README.md)
* **LinkedIn:** [[your-linkedin-profile](https://linkedin.com/in/your-linkedin-profile)](https://www.linkedin.com/in/niranjan-rathod?utm_source=share_via&utm_content=profile&utm_medium=member_android)

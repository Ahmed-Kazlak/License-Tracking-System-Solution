# 📊 License Tracking System Solution

A smart and scalable Power BI-based solution to help enterprises **track license usage**, **monitor user activity**, and **optimize software capacity utilization** through automated insights, user segmentation, and interactive dashboards.

---

## 🧠 Overview

This project provides a **comprehensive license monitoring system** by analyzing usage logs and capacity data to track:

- 🧍‍♂️ Internal user behavior  
- 🌐 External party license allocation  
- 📊 Enterprise-wide capacity planning

The report is broken down into **three main dashboards**:
1. **Internal**  
2. **External**  
3. **Capacity**

Each dashboard enables stakeholders to drill into details using filters like **email, location, job title, package, product, version**, and **date** to drive informed decisions.

---

## 🛠 Tools Used

| Tool               | Purpose                         |
|--------------------|----------------------------------|
| ⚡ Power BI         | Interactive dashboard & modeling |
| 🔗 Power Automate   | Scheduled refresh & data tracking |
| 🌀 Power Query      | Data transformation & merging     |
| 🧮 DAX              | Calculated measures & logic       |
| ☁️ SharePoint       | Central data storage              |
| 🔌 API              | Usage data extraction             |

---

## 🌐 Data Source

The solution integrates **three key data sources**:

1. 🧑‍💼 **Enterprise Control Center (Admin Account)**  
   - For real-time license usage and user logs  
2. 📄 **Capacity Sheet**  
   - Provides the total licensed capacity and assignments  
3. 📧 **Mails Sheet**  
   - Continuously updated list to filter out ex-employees

---

## 🧱 Data Modeling

- **Fact Table**
  - `Usage` → Core activity log including all usage metrics

- **Dimension Tables**
  - `Date` → Standard date table for time intelligence
  - `Mails` → Cleaned user profile and status
  - `Capacity` → License count and company quota

- **Calculated Tables**
  - `Efficiency Groups` → Users segmented into:
    - 0–25%  
    - 25–50%  
    - 50–75%  
    - 75–100%
  - `Utilization Groups` → Packages segmented into:
    - Underutilized (<50%)  
    - Moderate (50–80%)  
    - Overutilized (>80%)

---

## 🔍 Analysis Process

### Internal & External Dashboards:
- 📌 **KPIs:**  
  - Active users  
  - Avg. usage efficiency  
  - Package & product counts

- 📋 **Detailed Tables:**  
  - Usage breakdown by location, product, package, version  
  - Comprehensive user-level table with:
    - Email  
    - Location  
    - Job title  
    - Usage dates & duration  
    - Monthly average  
    - Efficiency %

- 📈 **Trends & Classifications:**  
  - Monthly usage trends  
  - Efficiency classification (0–100%)

- 🧰 **Interactive Filters:**  
  - Dynamic slicers for email, location, job title, version, etc.  
  - Clear filters button for user convenience

---

### Capacity Dashboard:
- 🏢 **Enterprise Metrics:**
  - Total capacity  
  - Assigned licenses  
  - Remaining licenses  
  - Utilization %

- 🧾 **Tables & Visuals:**
  - Package-level utilization details  
  - Top 10 external companies by usage  
  - License utilization chart in descending order  
  - Utilization classification (under/moderate/over)

- 🔀 **Distribution Breakdown:**  
  - Internal vs External usage

---

## 📌 Key Findings

- 🚫 Several users with low (0–25%) usage efficiency  
- 🔄 Some external companies heavily utilizing licenses  
- 💼 Certain packages are either underutilized or over-allocated  
- 📉 Opportunity to optimize assignments and reduce waste

---

## 💡 Conclusion

The **License Tracking System Solution** empowers enterprises to:
- Monitor actual license usage across stakeholders  
- Identify inefficiencies and reallocate resources  
- Maintain a clear view of license consumption vs capacity  
- Automate data collection and refresh pipelines

It bridges the gap between **IT governance** and **license performance visibility**, all in one intuitive Power BI solution.

---

## 📊 Dashboard Preview

> *(You can embed screenshots or GIFs of each dashboard here)*  
- `📌 Internal Dashboard`  
- `📌 External Dashboard`  
- `📌 Capacity Dashboard`

---

## 🔄 Automation

- Weekly API pulls scheduled via Power Automate  
- Usage data appended to SharePoint  
- Auto-refresh and update notifications enabled  

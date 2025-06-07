# 🛒 Order & Supplier Performance Dashboards – Power BI/ SQL/ Python/ Excel

This Power BI dashboard suite was created to track and optimize order lifecycle management and supplier service levels across Carrefour's apparel and merchandise departments. It provides deep visibility into milestones, delays, cancellations, and performance KPIs.

![CarreFour_Test_Dashboards_page-0001](https://github.com/user-attachments/assets/5d7c6921-a98b-4a36-a8d1-adbf3b7c0cdc)
![CarreFour_Test_Dashboards_page-0002](https://github.com/user-attachments/assets/16009fd3-6fd5-4eae-b810-c6d318f932bb)
![CarreFour_Test_Dashboards_page-0003](https://github.com/user-attachments/assets/402b30f0-7244-4b82-a12d-a367fbaa5b44)

---

## 🔍 Purpose

This dashboard was designed to:
- Monitor the **status and progression** of purchase orders by category, supplier, and merchandiser
- Track supplier **service level agreements** (SLAs) based on order delays and fulfillment
- Help buyers and managers identify **orders at risk** and take corrective action early
- Provide merchandisers a consolidated view of **late, upcoming, and closed orders**

---

## 🎯 Business Impact

- Improved **transparency and accountability** for over 23M+ order units
- Identified **979K+ cancelled orders** and **69M+ units at risk**, aiding recovery planning
- Enabled **supplier performance benchmarking** based on CRD (Committed Ready Date) adherence
- Facilitated faster resolution of production delays using milestone visualizations
- Empowered merchandiser and buyer managers to act on **late-not-closed orders** using role-based views

---

## 🛠️ How It Was Created

### 📊 Power BI
- **Data sources**: Excel/CSV and SQL dumps from Carrefour’s internal order systems
- **Dashboards developed**:
  - **Detailed Status Dashboard**: Tracks real-time progress by department, order, and milestone
  - **Milestone Tracker**: Displays merchandiser- and buyer-specific overdue and upcoming due dates
  - **Progression Dashboard**: Supplier-centric view for total orders, cancellations, approvals, and service metrics
- **Features used**:
  - DAX calculations for aggregating order counts per milestone
  - Slicers by department, supplier, merchandiser, buyer, category
  - Service level and delay % calculations by supplier

---

### 🐍 Python Integration

Python was used alongside Power BI for **data preprocessing** and **performance metric calculations**, especially when dealing with:
- Cleaning inconsistent milestone timestamps
- Flagging "late-not-closed" orders by comparing today's date with due dates
- Calculating CRD delay days per supplier for ranking performance
- Data enrichment (e.g., extracting quarters, flags for at-risk orders)

---

## 📌 Key Takeaways
- 23.5M+ units tracked across multiple dashboards
- ~1M orders cancelled, suggesting vendor or planning issues
- 69M+ units at risk, flagged for proactive intervention
- Worst-performing suppliers had >20 days delay on average
- Top 5 suppliers delivered ~75% on time, while bottom 5 had <5% service level
- Clear visibility for merchandisers and buyers into their portfolio performance

---

## 🧰 Tools Used
- Power BI:	Dashboarding, DAX calculations, interactivity
- Python:	Data cleaning, delay logic, SLA metrics
- Excel/CSV:	Source files for orders, milestones, and vendors
- SQL:	Backend integration for order management exports

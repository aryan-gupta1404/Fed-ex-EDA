# FedEx Logistics & Delivery Performance Analysis

## Project Overview

This project focuses on analyzing real-world FedEx shipment and delivery data to identify the major causes of delivery delays and operational inefficiencies. The analysis explores shipment modes, vendor performance, country-wise delivery trends, freight costs, and delivery timelines to generate business insights and actionable recommendations.

A new feature called `delay_days` was created to measure the difference between scheduled delivery dates and actual delivery dates, helping identify late, early, and on-time shipments.

---

## Business Problem

The company is facing several logistics-related challenges:

* Frequent delivery delays
* Poor delivery performance in certain regions
* Inefficient vendor performance
* High shipping costs
* Lack of visibility into delivery operations

The goal of this project is to use data analysis to improve logistics efficiency, reduce delays, optimize vendor selection, and support better operational decision-making.

---

## Business Objectives

* Reduce delivery delays
* Improve shipment efficiency
* Optimize freight costs
* Identify underperforming vendors
* Improve customer satisfaction
* Support data-driven logistics decisions

---

## Dataset Information

The dataset contains shipment-level information including:

* Shipment mode
* Vendor details
* Country/region
* Delivery dates
* Freight cost
* Shipment quantity
* Weight and insurance
* Line item values

Dataset Size:

* 10,324 rows
* 33 columns

---

## Tools & Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## Data Cleaning & Feature Engineering

The following preprocessing steps were performed:

* Handled missing values
* Converted date columns into datetime format
* Converted freight and weight columns into numeric datatype
* Created a new column:

```python
delay_days = Delivered Date - Scheduled Delivery Date
```

* Checked duplicates and null values
* Performed data type corrections

---

## Exploratory Data Analysis (EDA)

The project includes multiple visual analyses such as:

* Shipment mode distribution
* Country-wise delivery volume
* Country-wise average delivery delays
* Vendor-wise delay analysis
* Freight cost vs delivery delay analysis
* Shipment mode vs delay comparison

Visualization techniques used:

* Bar Charts
* Scatter Plots
* Comparative Analysis Charts

---

## Key Insights

### Shipment Mode Analysis

* Air shipment was the most commonly used shipment method.
* Truck shipments showed the highest average delivery delays.
* Ocean and Rail shipments appeared more cost-effective and stable for non-urgent deliveries.

### Country-Level Insights

* South Africa handled the highest number of deliveries.
* Congo, DRC showed the highest average delivery delays.
* Togo and Benin also experienced operational inefficiencies.

### Vendor Performance Insights

* The vendor `SCMS from RDC` consistently showed the highest delays across multiple countries.
* Removing this vendor from analysis significantly reduced average delay days in Congo, Togo, and Benin.
* Vendor performance had a major impact on overall delivery efficiency.

### Freight Cost vs Delay

* Higher freight cost did not always guarantee faster deliveries.
* Some vendors had both high freight costs and high delays, indicating inefficiencies.

---

## Business Recommendations

* Reassess partnerships with consistently underperforming vendors.
* Implement stricter vendor performance monitoring systems.
* Optimize shipment mode selection based on urgency and cost.
* Improve logistics planning in high-delay regions.
* Use data-driven vendor evaluation for future contracts.
* Focus operational improvements on truck-based logistics.

---

## Conclusion

This project demonstrates how exploratory data analysis can be used to solve real-world logistics and supply chain problems. The analysis successfully identified key operational bottlenecks, problematic vendors, and inefficient shipment strategies that contribute to delivery delays.

The findings can help businesses improve delivery performance, reduce operational costs, and make more informed logistics decisions.

---

## Project Structure

* `FedEx_EDA.ipynb` → Jupyter Notebook
* `README.md` → Project Documentation
* `SCMS_Delivery_History_Dataset.csv` → Dataset

---

## Author

Aryan Gupta

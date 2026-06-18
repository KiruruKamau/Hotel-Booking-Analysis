# Hotel Booking Demand Analysis
* An end_to_end data analysis project uncovring the drivers of hotel cancellations and seasonal booking trends. *

---

## Table of Contents
* [About the Project](#about-the-project)
* [Business Questions Answered](#business-questions-answered)
* [Data & Tech Stack](#data--tech-stack)
* [Visuals & Key Findings](#visuals--key-findings)
* [Getting Started](#getting-started)
* [Executive Recommendations](#executive-recommendations)

---

## About the Project
This project acts as a  strategic analysis for a simulated hotel chain. Using Kaggle "Hotel Booking Demand" dataset (119k+ records), the goal was to 
identify the root causes of cancellations, map out seasonal demand, and discover which customer segments provide the highest lifetime value.
This Analysis moves from raw data cleaning and feature engineering to deep exploratory data analysis.

---

# Business Questions Answered
1. What is the overall baseline cancellation rate?
2. Which property type (City Vs Resort) faces the highest volatility?
3. How does lead time (booking in advance) affect cancellation probability?
4. When are the peak booking seasons, how should pricing reflect this?
5. Which customer demographic generates the most reliable revenue?

---

## Data & Tech Stack
* **Dataset:** [Hotel Booking Demand on Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
* **Language:** Python 3
* **Libraries:** *`pandas`(Data manipulation and cleaning)
 * `numpy` (numerical computing)
 * `matplotlib` & `seaborn`(Data Visualisation)

---

## Visuals and Key Findings

### 1. The Impact of Lead Time on Cancellations
![Lead Time Analysis](https://github.com/KiruruKamau/Hotel-Booking-Analysis/blob/main/Images/leadtime.png)
> *Insight:* The longer the time between booking and arrival, the higher the chance of cancellation. Bookings made 90+ days in advance are highly volatile.

### 2. Seasonal Demand (Monthly Trends)
![Monthly Trends Bar Chart](https://github.com/KiruruKamau/Hotel-Booking-Analysis/blob/main/Images/monthlytrends.png)
> *Insight:* July and August are the peak demand months. The hotel has maximum pricing leverage during the European summer holidays.

### 3. Cancellations by Hotel Type
![Hotel Type Comparison](https://github.com/KiruruKamau/Hotel-Booking-Analysis/blob/main/Images/hoteltype.png)
> *Insight:* City Hotels experience significantly higher cancellation rates compared to Resort Hotels, likely due to shorter, easily alterable business trips or weekend getaways.

## Getting Started

To run this analysis on your local machine:

### Prerequisites
Ensure you have Python installed along with the required libraries.
```bash
pip install pandas numpy matplotlib seaborn jupyter
```
Installation
Clone the repository:

Bash
git clone [https://github.com/KiruruKamau/Hotel-Booking-Analysis](https://github.com/KiruruKamau/Hotel-Booking-Analysis)
Download the dataset from Kaggle and place hotel_bookings.csv in the root directory.

Open the Jupyter Notebook:

Bash
jupyter notebook hotel_analysis.ipynb

## Executive Recommendations
Based on the data analysis, the following actions are recommended to management:

Implement Aggressive Overbooking: Overbook City Hotels by 20-30% on weekends to counteract the >50% cancellation rate from local transient demographics.

Tiered Deposit Strategy: Enforce a 20% non-refundable deposit for any booking made more than 60 days in advance to mitigate the "lead time trap."

Targeted Marketing: Shift marketing spend toward Family segments, as they generate significantly higher Average Revenue Per Booking than solo travelers.

IT Systems Audit: Immediately investigate "Non Refundable" booking codes in the PMS system, as data indicates a near 100% cancellation rate on these blocks, suggesting a severe operational anomaly.






# Amazon.in Market Sizing (Guesstimate) Case Study

## Project Overview

The goal is to **estimate the daily volume of items sold on Amazon.in** by breaking down the Indian market into core consumption factors.  

The model is implemented in **Python**, allowing for quick testing and validation of different business assumptions.  

---

## Model Methodology (The 6 Steps)
The estimation follows a logical, step-by-step breakdown starting from the total market size:

1. **Estimate Total Households** – Establish the population base.  
2. **Internet Penetration** – Filter for households with internet access.  
3. **Amazon Adoption** – Filter for the subset of internet users who order from Amazon.in.  
4. **Order Frequency** – Estimate the average orders placed per active household per month.  
5. **Items per Order** – Estimate the average number of physical items in a single order.  
6. **Final Calculation** – Use these variables to calculate the total monthly items, then divide by 30 days to get the daily sales estimate.  

---

## Key Assumptions & Base Case

| Metric                                  | Value          | Unit                       |
|-----------------------------------      |----------------|----------------------------|
| **Total Households**                    | 300,000,000    | count                      |
| **Internet Penetration (internet_pct)** | 50% (0.50)     | ratio                      |
| **Amazon Adoption Rate (amazon_pct)**   | 20% (0.20)     | ratio (of internet HHs)    |
| **Orders / Household / Month**          | 2              | count                      |
| **Items / Order**                       | 3              | count                      |

---

## 📈 Base Case Result
The base calculation resulted in an estimate of:

> **✅ ~6,000,000 items sold per day on Amazon.in**

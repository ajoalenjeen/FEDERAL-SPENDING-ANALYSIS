# Federal-Spending-Analysis
# Overview:

A complete data-driven analysis of U.S. federal contract spending using Python, Pandas, Plotly, Matplotlib, and Seaborn.

This project investigates where U.S. federal money goes, which agencies and contractors receive the most funding, how concentration emerges, and which agencies pose the highest budget risk.

The analysis is based on ~2.5M+ federal contract records downloaded from USAspending.gov.

#### Agencies Included in This Analysis:

The project analyzes federal contract spending (2020–2024) across the following 14 awarding agencies:

* Department of Veterans Affairs (VA)

* Department of Energy (DOE)

* Department of Health and Human Services (HHS)

* Department of Homeland Security (DHS)

* Department of State (DOS)

* Department of Agriculture (USDA)
  
* Department of Justice (DOJ)

* Department of the Treasury

* Department of Transportation (DOT)

* Department of the Interior (DOI)

* Department of Commerce (DOC)

* Department of Education (ED)

* Department of Labor (DOL)

* Department of Housing and Urban Development (HUD)

# Dataset:
https://www.usaspending.gov/search?hash=0f5d91bedf605af1660a7326fd87a92f

# Analysis:

## What is total Contract spending by agency and fiscal year?

Total Federal Spending: $1,138.24B


Federal Contract Spending (2020–2024)
* FY2020: $198.59B
* FY2021: $211.84B
* FY2022: $228.34B
* FY2023: $246.69B
* FY2024: $252.77B


<img src="https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/d37ae06b474682ed69a9604161b617eaea4f5a03/Image/Screenshot%202025-11-25%20190704.png?raw=true" width="800">
 
* The Department of Veterans Affairs, Department of Energy, and Department of Health & Human Services accounted for the majority of the spending, reflecting national priorities in healthcare, energy infrastructure, and research. 
* Heatmap analysis shows clear year-over-year increases in VA and DOE spending, while HHS spending was elevated during COVID-19 years before stabilizing.

Overall, spending trends indicate growing investment in public health, national security, and technology modernization.


## Which contractors receive the most federal funding?

![image alt](https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/7f25ffe01e57fa0a96ced690db8d4fc73f0b06b4/Image/Screenshot%202025-11-25%20181729.png)

Federal contract spending is highly competitive, as shown by a very low HHI (0.0081).
However, a few vendors consistently dominate due to the government’s reliance on:

* Healthcare services & claims management (Optum, TriWest)

* Pharmaceutical distribution (McKesson)

* National laboratories & defense R&D (Sandia, Triad National Security)

Across FY2020-FY2024, health-related vendors receive the largest contract obligations, showing that public health, veterans’ services, and pandemic recovery remain top federal priorities.


## What drives spending concentration in certain states or sectors?

<img src="https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/7da77a4935b1b9d5203ba53726cbb97ef4a614ac/Image/newplot.png?raw=true" width="800">

<img src="https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/497a62e5fdb911bd69a6f0ffdd518380bdbeee88/Image/Screenshot%202025-11-25%20214321.png?raw=true" width="800">

The choropleth map shows that states such as Virginia, Texas, California, Maryland, and Florida capture a disproportionate share of federal contract spending.

The sector bar chart highlights the Top 10 NAICS industries receiving the most federal funds.


Federal contract spending from 2020–2024 exhibits strong geographic and structural concentration driven by agency operations, vendor dependency, and sector specialization rather than population or economic size alone.

### Key Drivers

**1. Agency mission and operational footprint**  
* Spending is concentrated in states hosting major federal infrastructure such as agency headquarters, hospitals, laboratories, and long-term facilities. 
* A small number of agencies dominate total obligations within top-spending states, reinforcing structural concentration.

**2. Vendor dependency and limited competition**  
* Vendor-level concentration analysis using the Herfindahl–Hirschman Index (HHI) reveals heavy reliance on a small number of contractors in several states. 
* Vendor HHI values exceed 3,000 in states such as New Mexico, Nevada, Idaho, and Kansas, indicating high market concentration and repeated awards to dominant vendors.

**3. Sector specialization**  
* Federal spending is concentrated in a narrow set of specialized industries, including facilities support services, healthcare and medical services, information technology, construction, and research and development.
* Sector HHI values exceed 7,300 in New Mexico and 4,400 in Tennessee, highlighting limited sector diversification within certain states.

**4. Large, high-value contracts**  
* A small number of high-value, multi-year contracts account for a significant share of total obligations. 
* These contracts amplify both vendor and sector concentration by outweighing numerous smaller awards.


##  How do contracts compare to grants in terms of dollar amounts and recipient concentration?

* Total Federal Spending (Contract): $1,138.24B
* Total Federal Spending (Grants): $6,073.20B

![image alt](https://github.com/ajoalenjeen/FEDERAL-SPENDING-ANALYSIS/blob/4e9c89ce0e1cd635b711292ec1699a8f7bb8b4df/Image/Screenshot%202026-01-19%20203145.png)

Federal grants vastly outweigh contracts in total spending, representing more than 80% of annual federal obligations from 2020–2024. Contracts remain a smaller portion, around 13–17% per year.

However, when comparing recipient concentration:

* Contracts (HHI = 0.0081) are moderately concentrated. A few major healthcare, and research contractors dominate (e.g., Optum, McKesson, TriWest, National Labs).

* Grants (HHI = 0.01613) are even more concentrated in this dataset. A relatively small number of large state governments, universities, and tribal authorities receive a disproportionate share of total grant dollars.


## Which agencies show the highest spending growth or budget risk?

Analysis of federal contract spending from 2020–2024 identifies clear differences across agencies in terms of spending growth and budget risk, measured using year-over-year (YoY) growth and spending volatility (coefficient of variation).

### Agencies with Highest Spending Growth
* The **Department of Housing and Urban Development (HUD)** shows the strongest growth profile, with an **average YoY growth rate of 23.51%**, indicating rapid expansion in contract obligations. 
* Other agencies with notable average growth include the **Department of the Interior (16.03%)**, **Department of Veterans Affairs (13.85%)**, and the **Department of the Treasury (10.92%)**, suggesting sustained increases in spending over the period.

### Agencies with Highest Budget Risk
Budget risk is highest among agencies exhibiting both strong growth and high spending volatility. HUD ranks highest in relative risk, with a **coefficient of variation (CV) of 35.12%**, indicating large year-to-year fluctuations relative to its average spending level. The **Department of the Interior (CV ≈ 24.95%)** and the **Department of Veterans Affairs (CV ≈ 19.78%)** also show elevated risk, reflecting exposure to program-driven or project-based funding cycles. In contrast, agencies such as **Health and Human Services (CV ≈ 4.34%)** and **Justice (CV ≈ 5.69%)** demonstrate more stable spending patterns despite large absolute budgets.

### Overall Assessment
Agencies such as HUD, Interior, and Veterans Affairs warrant closer budget monitoring due to their combination of rapid spending growth and high volatility. These patterns suggest greater exposure to funding uncertainty and execution risk, while agencies with lower volatility exhibit more predictable and stable contract spending profiles.


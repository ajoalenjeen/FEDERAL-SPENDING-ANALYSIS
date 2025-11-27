# Federal-Spending-Analysis
# Overview:

A complete data-driven analysis of U.S. federal contract and grant spending using Python, Pandas, Plotly, Matplotlib, and Seaborn.

This project investigates where U.S. federal money goes, which agencies and contractors receive the most funding, how concentration emerges, and which agencies pose the highest budget risk.

The analysis is based on ~2.5M+ federal contract and grant records downloaded from USAspending.gov.

# Analysis

## What is total spending by agency and fiscal year?

Total Federal Spending: $1,138.24B


Federal Contract Spending (2020–2024)
* FY2020: $198.59B
* FY2021: $211.84B
* FY2022: $228.34B
* FY2023: $246.69B
* FY2024: $252.77B

![image alt](https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/f8f023fa103ef27460f8e3baedc106ff97844d04/Image/Screenshot%202025-11-25%20190652.png)

![image alt](https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/d37ae06b474682ed69a9604161b617eaea4f5a03/Image/Screenshot%202025-11-25%20190704.png)

Federal contract spending steadily increased from FY2020 to FY2024, rising from $198.6B to $252.8B. The Department of Veterans Affairs, Department of Energy, and Department of Health & Human Services accounted for the majority of the spending, reflecting national priorities in healthcare, energy infrastructure, and research. Heatmap analysis shows clear year-over-year increases in VA and DOE spending, while HHS spending was elevated during COVID-19 years before stabilizing. Overall, spending trends indicate growing investment in public health, national security, and technology modernization.


## Which contractors receive the most federal funding?

![image alt](https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/7f25ffe01e57fa0a96ced690db8d4fc73f0b06b4/Image/Screenshot%202025-11-25%20181729.png)

Federal contract spending is highly competitive, as shown by a very low HHI (0.0081).
However, a few vendors consistently dominate due to the government’s reliance on:

* Healthcare services & claims management (Optum, TriWest)

* Pharmaceutical distribution (McKesson)

* National laboratories & defense R&D (Sandia, Triad National Security)

Optum Public Sector Solutions emerges as the largest contractor starting FY2021, reflecting growth in federal health analytics, Medicare/Medicaid data systems, and VA healthcare management.

Across FY2020-FY2024, health-related vendors receive the largest contract obligations, showing that public health, veterans’ services, and pandemic recovery remain top federal priorities.


## What drives spending concentration in certain states or sectors?

![image alt](https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/60cf5a2b95f1e3e23ade336b9922e890662648f3/Image/newplot.png)
The choropleth map shows that states such as Virginia, Texas, California, Maryland, and Florida capture a disproportionate share of federal contract spending.

1. Virginia (VA) leads even without DoD data

Virginia remains the highest-spending state because:

It hosts major federal contracting hubs in Northern Virginia (Arlington, Fairfax, Reston, Chantilly).

Home to large contractors serving civilian agencies
(e.g., Booz Allen, SAIC, Leidos, GDIT, Accenture Federal).

Many contracts are for IT modernization, cybersecurity, logistics, and healthcare support.

✔ Conclusion: Spending is concentrated where federal contractors are physically located.

2. Texas (TX) and California (CA) also show significant spending

These states contain:

Major federal hospitals (VA medical centers)

Large research laboratories (DOE & NIH grantees)

Border security operations (DHS)

Strong biotechnology & technology ecosystems

✔ Conclusion: States with major infrastructure, medical facilities, or tech ecosystems naturally receive higher obligations.

3. Rural or low-population states receive less

States without:

Large federal labs

Advanced tech industries

![image alt](https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/497a62e5fdb911bd69a6f0ffdd518380bdbeee88/Image/Screenshot%202025-11-25%20214321.png)

The sector bar chart highlights the Top 10 NAICS industries receiving the most federal funds.

The biggest sectors include:

Facilities Support Services

Health and Medical Insurance Carriers

Computer Systems Design Services

Other Computer-Related Services

Pharmaceutical & Medical Manufacturing

Research & Development Services

1. Healthcare dominates due to VA + HHS

The federal government is the largest healthcare purchaser in the U.S., so spending is concentrated in:

Medical supplies & pharmaceuticals

Diagnostics & laboratory services

Health insurance processing

Hospital facility operations

✔ Conclusion: Healthcare spending is structurally high because VA and HHS rely heavily on private contractors.

2. IT Services rank among the top sectors

Civilian agencies (Treasury, Commerce, HUD, Education, DHS, State) all require:

Cybersecurity

Cloud migration

Data center operations

Software development

Network modernization

✔ Conclusion: Federal IT modernization mandates drive massive spending in IT and computer-related services.

3. Facility maintenance & construction are major recurring costs

All federal agencies require:

Building operations

Laboratory upkeep

Real estate services

Infrastructure support

✔ Conclusion: Facilities support is a large cost center across all agencies.


##  How do contracts compare to grants in terms of dollar amounts and recipient concentration?

Total Federal Spending: $1,138.24B
Total Federal Spending: $5,570.54B

![image alt](https://github.com/ajoalenjeen/Federal-Spending-Analysis/blob/10f0a4e9eea851bf32544006945bb8dd53eb3268/Image/Screenshot%202025-11-26%20161315.png)

Federal grants vastly outweigh contracts in total spending, representing more than 80% of annual federal obligations from 2020–2024. Contracts remain a smaller portion, around 14–18% per year.

However, when comparing recipient concentration:

Contracts (HHI = 0.0081) are moderately concentrated. A few major defense, healthcare, and research contractors dominate (e.g., Optum, McKesson, TriWest, National Labs).

Grants (HHI = 0.01499) are even more concentrated in this dataset. A relatively small number of large state governments, universities, and tribal authorities receive a disproportionate share of total grant dollars.

Conclusion:

Even though grants represent far more total dollars, both contracts and grants show measurable concentration — but grants are more concentrated than contracts in this dataset. This suggests much of federal grant money flows to a smaller number of very large public-sector and nonprofit institutions.

Major healthcare networks

Federal logistics hubs

tend to receive much smaller contract amounts.

## Which agencies show the highest spending growth or budget risk?


Federal contract spending growth and volatility reveal which agencies pose the highest budget risk between FY 2020–2024.

Highest Growth Agencies

HUD (+101%) — largest single-year explosion in spending.

Education (+13.7%), VA (+8.4%), Energy (+6.5%) — strong consistent increases.

Highest Volatility Agencies (Budget Risk)

Veterans Affairs ($11.18B volatility) — healthcare, medical supply, hospital infrastructure.

Energy ($4.95B) — large-scale R&D, national labs, nuclear programs.

Homeland Security ($2.19B) — disaster response and emergency spikes.

Interior ($1.71B) — fire management, environmental emergencies.

HHS ($1.57B) — massive pandemic-related fluctuations.

Most At-Risk Agencies (Combined Growth + Volatility)

HUD — extreme growth + emerging instability

Education — early signs of sharp spending increase

Veterans Affairs — high volatility + strong growth

Energy — large infrastructure-driven risk

Commerce — rising spending + medium volatility

Conclusion:
HUD and VA emerge as the agencies with the highest spending expansion and volatility, making them the primary sources of budget risk in the 2020–2024 contracting landscape.

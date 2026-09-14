# SCA-Capstone-Health-Geographic-Patterns
Power BI capstone project analyzing regional health service utilisation patterns across 40 facilities in Nigeria — SCA Technical Deep Dive 3.0, Project 2D
# Geographic Health Patterns — Power BI Capstone Project

**SCA Technical Deep Dive 3.0 | Capstone Project 2D**
**Author:** Zainab Muhammad Nasir
**Cohort 3 | Internal Defence: 15 September 2026**

## Business Problem

Health service utilisation and facility performance vary across regions, but the state health programme lacks a consolidated, region-level view of where demand is highest, which facilities and services drive regional differences, and where resource-planning gaps exist. This project analyzes patient visit data to uncover these geographic patterns and support more equitable resource allocation.

## Dataset

- ~25,000 patient visit records
- 40 health facilities across 4 regions (North East, North Central, North West, South West)
- Reporting period: January 2024 – August 2026
- Includes facility, patient, and service reference data

## Analytical Questions

1. Which regions have the highest and lowest utilisation?
2. Which facilities/services drive regional differences?
3. Are there notable geographic imbalances?
4. How do regional patterns change over time?

## Methodology

- **Data cleaning (Power Query):** Removed duplicate visit records; handled missing wait-time and cost values
- **Data modelling:** Built a star schema (Health_Visits_FACT connected to Facilities, Patients, Services, and a dedicated Date dimension table)
- **DAX measures:** Total Visits, Unique Patients, Average Wait Time, Average Cost, Referral Rate %
- **Analysis:** Compared regions on utilisation, facility count, service mix, cost, wait time, and monthly trends

## Key Insights

1. North East's higher visit volume (14,578) is explained entirely by operating 13 facilities — 4 more than any other region
2. Visits per facility are nearly identical across all regions (1,087–1,130)
3. Service mix is proportionally consistent across all regions (no region has distinct care needs)
4. Visit volumes are stable over time in every region (2024–2026)
5. Wait times and costs are virtually uniform system-wide

## Recommendations

1. Review facility distribution across regions to match coverage with population/demand
2. Maintain current staffing and resourcing models, since demand is consistent per facility nationwide
3. Investigate the absence of facilities in South East and South South zones

## Files in This Repository

- `Zainab_Muhammad_Nasir_Capstone.pbix` — Power BI project file
- `Zainab_Muhammad_Nasir_Capstone_Defence_Deck.pptx` — Defence presentation

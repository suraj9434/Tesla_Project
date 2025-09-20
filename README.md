

# Tesla in Washington: Market Share, Sales, and EV Landscape

**Author:** Suraj Shrestha

### [**View the Live Dashboard on RPubs**](https://rpubs.com/surajshrestha7494/1346455)



## Project Overview

This project provides an executive-level analysis of Tesla's electric vehicle (EV) market presence in Washington state. Using public data on EV registrations, this report answers key business questions about market share, top-selling models, competitive positioning, and consumer trends. The goal is to deliver data-driven insights and actionable recommendations to support Tesla's strategic decisions in the region.

The final output is a `flexdashboard` report designed for a business audience, focusing on clear visualizations and concise summaries.

## Business Case Scenario

This analysis was developed to fulfill a request for a **Tesla Executive Briefing**. The primary task was to analyze the Washington state EV dataset to answer the following high-priority questions:

1.  What percentage of EVs in Washington are Teslas?
2.  Which Tesla models sell the most, and what is the estimated revenue from these sales?
3.  How does Tesla compare to its competitors on key metrics like range and MSRP?
4.  What are the market adoption trends for Battery Electric Vehicles (BEVs) versus Plug-in Hybrid Electric Vehicles (PHEVs)?
5.  Which electric utility providers serve the largest number of Tesla owners in Washington?

The deliverable needed to present key figures and visualizations in an easily digestible format for executive review.

## Key Insights & Visualizations

*(All visualizations can be viewed in the [live dashboard](https://rpubs.com/surajshrestha7494/1346455).)*

#### 1. Market Share: Tesla's Dominance
A pie chart illustrates that Tesla commands a significant **~30.4%** of the EV market in Washington, highlighting its strong brand presence and leadership over other manufacturers.

#### 2. Sales Performance: Models and Revenue
-   **Units Sold:** A bar chart shows the **Model 3** and **Model Y** as the top-selling models, indicating a strong preference for Tesla's more accessible vehicles.
-   **Estimated Revenue:** A separate bar chart reveals that despite lower unit sales, the higher-priced **Model Y** and **Model S** are major revenue drivers, showcasing a successful dual strategy of targeting both volume and high-margin segments.

#### 3. Sales Trends: Consistent Growth
A line chart tracks Tesla sales year-over-year, showing consistent growth that peaked after the mass-market introduction of the Model 3. This trend mirrors the broader adoption of EVs in the state.

#### 4. Competitive Landscape: Range vs. Price
-   **Electric Range:** A bar chart compares the average electric range of Tesla vehicles against other BEVs, demonstrating Tesla's significant competitive advantage.
-   **MSRP:** Another bar chart compares the average MSRP, showing that consumers are willing to pay a premium for the Tesla brand and technology.

#### 5. Market Trends: BEV vs. PHEV
A line chart visualizes the market shift towards **BEVs over PHEVs**, a trend that directly benefits Tesla's all-electric lineup.

#### 6. Customer Demographics: Utility Providers
A bar chart highlights that a large concentration of Tesla owners are customers of a few major utilities, primarily **Puget Sound Energy** and **City of Seattle**, pointing to clear opportunities for partnership.

## Summary of Findings & Recommendations

#### **Findings**
-   Tesla dominates Washington’s EV market with **~30.4%** share.
-   **Model 3 and Model Y lead sales**, but Model Y and S contribute disproportionately high revenue.
-   **Tesla vehicles outperform competitors** in average range, solidifying their technological edge.
-   The market's rapid **shift toward BEVs** strongly favors Tesla’s product strategy.
-   Tesla ownership is highly concentrated within the service areas of a few key utility companies.

#### **Recommendations**
-   **Strengthen Utility Partnerships:** Collaborate with Puget Sound Energy and City of Seattle on charging infrastructure, smart grid programs, and joint marketing initiatives.
-   **Optimize Model Strategy:** Continue to push the Model Y to capture demand for both high-volume and high-revenue vehicles.
-   **Leverage Range Advantage:** Emphasize Tesla's superior range in regional marketing campaigns to address consumer range anxiety.
-   **Monitor BEV Policy:** Actively track and engage with state-level policy incentives in Washington to maintain a competitive edge.
-   **Explore Affordability:** Develop strategies or financing options to make Tesla ownership more accessible and further expand the customer base.

## Data Sources

1.  **Electric Vehicle Population Data (Washington State)**
    -   **Source:** data.gov
    -   **Link:** [https://catalog.data.gov/dataset/electric-vehicle-population-data](https://catalog.data.gov/dataset/electric-vehicle-population-data)
    -   **Note:** This dataset covers registrations from 2008 to March 2025.

2.  **Tesla Current Base Prices**
    -   **Source:** GitHub Repository (Curated List)
    -   **Link:** [https://raw.githubusercontent.com/suraj9434/Tesla_Project/refs/heads/main/Tesla_Current_Base_Prices.csv](https://raw.githubusercontent.com/suraj9434/Tesla_Project/refs/heads/main/Tesla_Current_Base_Prices.csv)
    -   **Note:** This data was used to supplement incomplete MSRP information in the primary dataset.

## Tools and Technologies

-   **Language:** R
-   **IDE:** RStudio
-   **Core Libraries:**
    -   `flexdashboard`: For creating the interactive dashboard.
    -   `dplyr` & `tidyverse`: For data manipulation and wrangling.
    -   `ggplot2`: For creating static visualizations.
    -   `readr`: For loading CSV data.
    -   `scales`: For formatting labels in plots (e.g., currency, percentages).

## How to Reproduce this Analysis

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    ```
2.  **Download the data:**
    -   Download the `Electric_Vehicle_Population_Data.csv` from the data.gov link above.
    -   Download the `Tesla_Current_Base_Prices.csv` from the GitHub link.
    -   Place both `.csv` files in your project directory.

3.  **Install R packages:**
    Open R or RStudio and run the following command in the console:
    ```r
    install.packages(c("flexdashboard", "dplyr", "tidyr", "tidyverse", "ggplot2", "scales", "readr", "stringr"))
    ```
4.  **Run the analysis:**
    -   Open the `.Rmd` file in RStudio.
    -   Update the file paths in the `read_csv()` functions to point to your downloaded data.
    -   Click the "Knit" button to generate the flexdashboard report.

## Notes and Limitations

-   The primary dataset includes vehicle registrations up to **March 2025**. Data for 2024 and 2025 may be incomplete.
-   The `Base MSRP` column in the original dataset had significant missing values. The analysis was supplemented with external data for Tesla models to estimate revenue, but competitor MSRP analysis may be skewed.

# Social-Media-Ad-Campaign

Overall, the data has 1143 entries and 11 columns. A brief description for each column can be given as follows:

ad_id: a unique ID for each ad.

xyzcampaignid: an ID associated with each ad campaign of XYZ company.

fbcampaignid: an ID associated with how Facebook tracks each campaign.

age: age of the person to whom the ad is shown.

gender: gender of the person to whom the add is shown

interest: a code specifying the category to which the person’s interest belongs (interests are as mentioned in the person’s Facebook public profile).

Impressions: the number of times the ad was shown.

Clicks: number of clicks on for that ad.

Spent: Amount paid by company xyz to Facebook, to show that ad.

Total conversion: Total number of people who enquired about the product after seeing the ad.

Approved conversion: Total number of people who bought the product after seeing the ad.

# Using Tools : Python(using libraries pandas, matlpotlib and seaborn)

# Overview

This project analyzes social media advertising campaigns to evaluate channel performance, audience engagement, and cost efficiency. The objective is to maximize ROI and provide data-driven recommendations for future ad budget allocations.

# Methodology :
- It was observed that some entries (207 entries) had both 'Spent' and 'Clicks' equal to 0. This is illogical for campaign performance analysis because if no money was spent and no users clicked, the record does not contribute any value to understanding ROI, CTR, or CPA. Therefore, these entries were removed, and our final dataset now consists of 936 entries.

# Analysis
- Data Cleaning: Removed illogical entries (e.g., zero clicks with positive conversions or zero clicks with zero spent).
- KPI Evaluation: Measured CTR, CVR, CPL, and CPA across demographics.
- Demographic Insights: Identified high-performing age groups **(30–34)** ,gender segments **(Male)**, interest **(31,36,101,102,112)**.
- Budget Reallocation: Suggested shifting investment toward efficient demographics with lower CPA and higher CVR.

# Visualization: 
Created heatmaps and comparative charts for performance insights.

# Key Insights
- Age 30–34 drives highest conversions with strong ROI.
- Male audience shows better efficiency (lower CPA, higher CVR).
- Budgets should prioritize these segments for maximum ROI.

# Future Budget Reallocation Strategy
- **Double down** on **Males, age 30–34, top 5 interests(31,36,101,102,112)** → this combo gives **lowest CPA**.
- Reduce waste on Females 45–49 and low ROI interests (>70 CPA).
- A/B test creatives for 35–44 group + mid-tier interests to see if CPA can be lowered.
- Monitor CPA trend monthly; reallocate dynamically based on performance shifts.


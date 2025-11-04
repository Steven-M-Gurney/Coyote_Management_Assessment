# Wildlife exclusion and management assessment: a coyote case study

### [Steven Gurney](https://linktr.ee/stevenmgurney), [Austin Messing](), [Selena Creed]()

### Manuscript: Special Publication No. 25-01 (2025). Wayne County Airport Authority, Airfield Operations – Wildlife Division, Detroit, MI, USA.

### Data: Most data are security sensitive and housed with the Wildlife Division's special-publication repository.

#### Please contact the first author for questions about the code or data: Steven M. Gurney (steven.m.gurney@gmail.com)
__________________________________________________________________________________________________________________________________________

## Summary

Detroit Metropolitan Wayne County Airport (DTW) is committed to maintaining the highest standards of aviation safety, security, and operational efficiency. In alignment with 14 CFR § 139.337 and DTW’s Wildlife Hazard Management Plan, proactive identification and mitigation of wildlife hazards are essential to reducing strike risks and protecting both airfield operations and the traveling public. Coyotes (Canis latrans) have emerged as a persistent and adaptable hazard at DTW, capable of breaching perimeter defenses and posing threats to safety, security, and airfield operations. Recognizing the importance of this issue, the Wayne County Airport Authority’s (WCAA) Airfield Operations – Wildlife Division spearheaded a systematic evaluation of coyote activity and perimeter vulnerabilities, providing actionable exclusion strategies informed by empirical data. The findings and recommendations presented in this report support DTW’s ongoing commitment to collaborative, science-based, adaptive wildlife hazard management. 

## Repository Directory

### [Integrated data analysis](./Integrated_Data_Analysis): Contains code for integrating, analyzing, and visulizing data.
* [Data_Integration.R](./Integrated_Data_Analysis/Data_Integration.R) - Code to process and integrate data from multiple sources.
* [Plots.R](./Integrated_Data_Analysis/Plots.R) - Code to visualize integrated-data results and produce control chart.

### [Spatial analysis](./Spatial_Analysis): Contains code for mapping, summarizing, and ranking sites problematic to exclusion.
* [Spatial_Data.R](./Spatial_Analysis/Spatial_Data.R) - Code to process and visualize landcover data; and calculate percent natural cover per buffered area.
* [Ranking_Summary.R](./Spatial_Analysis/Ranking_Summary.R) - Code to 1) rank priority level of sites problematic to exclusion (based on landcover and perimeter-survey data) and produce summary statistics.

### [Species hazard ranking](./Species_Hazard_Ranking): Contains code to process strike data and rank relative hazard level of species.
* [Species_Ranking.R](./Species_Hazard_Ranking/Species_Ranking.R) - Code to process data exported from the FAA strike database.
* [Strike_Data_Prep.R](./Species_Hazard_Ranking/Strike_Data_Prep.R) - Code to analyze strike metrics and produce relative hazard results by species.

# Wildlife Exclusion and Management Assessment:<br>A Coyote Case Study

### [Steven Gurney](https://linktr.ee/gurneyst), [Austin Messing](), [Selena Creed]()

### Manuscript: Wayne County Airport Authority<br>Airfield Operations, Wildlife Division<br>Special Publication No. 25-01

This repository includes code for wrangling, cleaning, analyzing, and visualizing data associated with the DTW Coyote Project. Most data are security sensitive and housed with the DTW Wildlife Team's special-publication repository.



# Harvest restrictions fail to influence population abundance

, [Sonja A. Christensen](http://www.christensen-lab.org/), [Melissa J. Nichols](), [Chad M. Stewart](), [David M. Williams](), [Sarah L. Mayhew](), [Neil A. Gilbert](https://gilbertecology.com), [Dwayne R. Etter]()

### Manuscript: [Published in Ecosphere](https://doi.org/10.1002/ecs2.70358)

### Data/code DOI: [![DOI](https://zenodo.org/badge/678437269.svg)](https://doi.org/10.5281/zenodo.15716493)

#### Please contact the first author for questions about the code or data: Steven M. Gurney (steven.m.gurney@gmail.com)
__________________________________________________________________________________________________________________________________________

## Abstract

Evaluating changes in population abundance is essential to assess the efficacy of conservation actions. Antler point restrictions are a high-profile regulatory action aimed to advance male age structure in cervid populations, but there is a limited understanding on how restrictions affect population size and structure. Our study evaluated population-level effects of an antler point restriction on white-tailed deer (*Odocoileus virginianus*) abundance and sex and age composition using a before-after control-impact design. Antler point restrictions are intended to increase the abundance of legal-antlered deer, but the impact on the abundance of antlerless deer is less known. By limiting the harvest of yearling males, antler point restrictions may lead hunters to shift harvest toward antlerless deer, potentially increasing female mortality and reducing population fecundity. We conducted camera-trap surveys of deer in zones with and without antler point restrictions before and three years after the implementation of restrictions and used N-mixture models to estimate annual abundance by sex and age class. The restriction prohibited the harvest of antlered deer with fewer than four points on a single antler beam (i.e., on one side). Our results suggest that the restrictions did not influence population abundance of deer. Abundance of legal-antlered deer increased in both the restriction zone and non-restriction zone (opposing predictions), as did the abundance of females, sublegal-antlered deer, and fawns (opposing predictions). Partial controllability, or a failure of the regulation to influence realized harvest, likely explains these results, since antlerless deer harvest did not change throughout the duration of our study while slight but insignificant change in antlered harvest was observed in the restriction zone. Our results highlight potential limitations of antler point restrictions achieving desired effects for population reduction goals and the importance of independently evaluating conservation and management actions.


## Repository Directory

### [Code](./Code): Contains code for preparing study data and running study model.
*  [Data_Prep](./Code/Data_Prep) - Folder with code to prepare study data for use in the N-mixture model.
   * [Data_Processing.R](./Code/Data_Prep/Data_Processing.R) - Code to process wrangled data.
   * [Data_Wrangling.R](./Code/Data_Prep/Data_Wrangling.R) - Code to wrangle study data.
* [N_Mixture_Model_Supplement.R](./Code/N_Mixture_Model_Supplement.R) - Code to fit alternative model with year as a factor rather than linear effect
* [N_Mixture_Model.R](./Code/N_Mixture_Model.R) - Code to fit N-mixture models (main text)

### [Data](./Data): Contains data for study.
*  [Count_Data](./Data/Count_Data) - Folder with verified count data by sex-and-age class and year (2019 - 2022; CSV files). These detection histories include a column for LocationName (unique name of sampling site, synonymous with SiteID) and columns associated with 9 seperate weekly counts.
   * [Counts_Fawns_2019.csv](./Data/Count_Data/Counts_Fawns_2019.csv) - Fawn count data for 2019.
   * [Counts_Fawns_2020.csv](./Data/Count_Data/Counts_Fawns_2020.csv) - Fawn count data for 2020.
   * [Counts_Fawns_2021.csv](./Data/Count_Data/Counts_Fawns_2021.csv) - Fawn count data for 2021.
   * [Counts_Fawns_2022.csv](./Data/Count_Data/Counts_Fawns_2022.csv) - Fawn count data for 2022.
   * [Counts_Females_2019.csv](./Data/Count_Data/Counts_Females_2019.csv) - Female count data for 2019.
   * [Counts_Females_2020.csv](./Data/Count_Data/Counts_Females_2020.csv) - Female count data for 2020.
   * [Counts_Females_2021.csv](./Data/Count_Data/Counts_Females_2021.csv) - Female count data for 2021.
   * [Counts_Females_2022.csv](./Data/Count_Data/Counts_Females_2022.csv) - Female count data for 2022.
   * [Counts_Legal_2019.csv](./Data/Count_Data/Counts_Legal_2019.csv) - Legal-antlered count data for 2019.
   * [Counts_Legal_2020.csv](./Data/Count_Data/Counts_Legal_2020.csv) - Legal-antlered count data for 2020.
   * [Counts_Legal_2021.csv](./Data/Count_Data/Counts_Legal_2021.csv) - Legal-antlered count data for 2021.
   * [Counts_Legal_2022.csv](./Data/Count_Data/Counts_Legal_2022.csv) - Legal-antlered count data for 2022.
   * [Counts_Sublegal_2019.csv](./Data/Count_Data/Counts_Sublegal_2019.csv) - Sublegal-antlered count data for 2019.
   * [Counts_Sublegal_2020.csv](./Data/Count_Data/Counts_Sublegal_2020.csv) - Sublegal-antlered count data for 2020.
   * [Counts_Sublegal_2021.csv](./Data/Count_Data/Counts_Sublegal_2021.csv) - Sublegal-antlered count data for 2021.
   * [Counts_Sublegal_2022.csv](./Data/Count_Data/Counts_Sublegal_2022.csv) - Sublegal-antlered count data for 2022.
*  [Covariate_Tables](./Data/Covariate_Tables) - Folder with annual covatiate tables (2019 - 2022; CSV files). These tables contain the following columns:
    | Variable name | Meaning |
    |---------------|---------|
    | SiteID | Unique name of sampling site |
    | ClosedCover | Binary indicator for dominant land cover, open (1) or closed (0) |
    | AgCover | Percent agricultural cover |
   * [CovariateTable_2019.csv](./Data/Covariate_Tables/CovariateTable_2019.csv) - 2019 covariate table.
   * [CovariateTable_2020.csv](./Data/Covariate_Tables/CovariateTable_2020.csv) - 2020 covariate table.
   * [CovariateTable_2021.csv](./Data/Covariate_Tables/CovariateTable_2021.csv) - 2021 covariate table.
   * [CovariateTable_2022.csv](./Data/Covariate_Tables/CovariateTable_2022.csv) - 2022 covariate table.

### [Figures](./Figures): Contains figures and code to create them.
*  [Code_For_Figures](./Figures/Code_For_Figures) - Folder with scripts and data to create figures.
   * [Figure_02.R](./Figures/Code_For_Figures/Figure_02.R) - Create Figure 2 (marginal effects).
   * [Figure_03.R](./Figures/Code_For_Figures/Figure_03.R) - Create Figure 3 (differences in abundance).
   * [Figure_04.R](./Figures/Code_For_Figures/Figure_04.R) - Create Figure 4 (harvest estimates).
   * [Figure_Supplement.R](./Figures/Code_For_Figures/Figure_Supplement.R) - Create supplemental figures visualizing results for model with year as a factor.
*  [Appendix_S2_Figure_S1.png](./Figures/Appendix_S2_Figure_S1.png) - Appendix S2: Figure S1. Marginal effects of year by harvest treatment (for supplemental model with year as a factor).
*  [Appendix_S2_Figure_S2.png](./Figures/Appendix_S2_Figure_S2.png) - Appendix S2: Figure S2. Differences in abundance between 2022 and 2019 (for supplemental model with year as a factor).
*  [Figure_01.tif](./Figures/Figure_01.tif) - Figure 1. Study area (created in ArcGIS Pro).
*  [Figure_02.tif](./Figures/Figure_02.tif) - Figure 2. Marginal effects of year by harvest treatment.
*  [Figure_03.tif](./Figures/Figure_03.tif) - Figure 3. Differences in abundance between 2022 and 2019.
*  [Figure_04.tif](./Figures/Figure_04.tif) - Figure 4. MDNR estimated deer harvest.
*  [Silhouette_Fawn.png](./Figures/Silhouette_Fawn.png) - Fawn silhouette for figure annotations.
*  [Silhouette_Sublegal.png](./Figures/Silhouette_Sublegal.png) - Sublegal antlered silhouette for figure annotations.
*  [Silhouette_Female.png](./Figures/Silhouette_Female.png) - Female deer silhouette for figure annotations.
*  [Silhouette_Legal.png](./Figures/Silhouette_Legal.png) - Legal antlered silhouette for figure annotations.

### [Results](./Results): Contains results files.
*  [Differences](./Results/Differences) - Folder with results from the interpretation model for difference in abundances (2022 - 2019; by sex-and-age class). These tables contain the following columns:
    | Variable name | Meaning |
    |---------------|---------|
    | trt | Harvest-treatment index (1 = Non-APR; 2 = APR)|
    | mean | Mean estimate of difference |
    | l95 | Lower credible interval of difference estimate |
    | u95 | Upper credible interval of difference estimate |
    | trt_name | Harvest-treatment acronym (Non=APR = no restrictions; APR = restrictions) |

# Research on San Francisco Climate Gentrification

Haoyu Yue, Urban Design and Planning, University of Washington

## Introduction

Based on numerous research, green infrastructure investments, such as green space, utilities, resilience infrastructure, green building adaptation, could contribute to the city and realize the green objectives while leading to green gentrification and increasing social inequity.

Even it is clear that *California Climate Investment* will lead to some negative effects on the disadvantaged and low-income communities, we cannot reject using them or stop investing in these communities. Here is a paradox between equity and efficiency. To understand the impact of investment and to make the trade-off, it is essential to identify which communities the green gentrification happened, what characteristics these communities have, what kind of green infrastructure investments lead to what degree of gentrification on communities.

## Research Question

- Does green infrastructure gentrification happen in San Francisco Bay Area caused by the California Climate Investments?

- How do the various types of climate investment impact different communities spatially?

## Data

- American Community Survey (ACS) Dataset - [Data Source](https://www.census.gov/programs-surveys/acs/data.html)
  
  - The dataset regularly gathers various information, such as ancestry, citizenship, educational attainment, income, language proficiency, migration, disability, employment, and housing characteristics.

- California Climate Investment Project Data - [Data Source](https://webmaps.arb.ca.gov/ccimap)
  
  - The dataset includes project-level information on California Climate Investments using Cap-and-Trade auction proceeds. The detailed project information includes location, program classification, year, funding amount, carbon emission reduction.

- Zillow's Housing Price Data - [Data Source](https://documenter.getpostman.com/view/9197254/SzRuZCCj?version=latest#2f82c962-5d77-40c2-bfcf-9f1a7e195afe)
  
  - A large dataset containing dozens of housing market metrics available at the national down to neighborhood level.

## Methodology

I will construct two indicators, *Green Gentrification Index* and *Infrastructure Investment Intensity Index* for each census tract within the research area (SF bay area). Then, try to understand the relationship between investments and gentrification based on statistical methods. Finally, visualize the result by Python.

![](https://lh6.googleusercontent.com/wqCCSWA-qrxlX6bePFb0YDcZdG0R6B44O-_K3DaMRiIwAalVzmzeNyjI-_zvDQX3KNyasF1hQJRRmVO9pVrQDT9Pn0diA77zeSDt4AKOXyEXLfT-JdfuZ5RL5DF_7zYUmKGTC9326Hda)

*Figure 1 Methodology Overview*

- Infrastructure Investment Index
  
  - Classify the project based on two categories
    
    - sectors (transportation, green space, air quality, etc.)
    
    - types(infrastructure/services, capital investment/non-capital investment etc.)
  
  - Distribute the investment into census block group based on the amount and distance. 

![](https://lh4.googleusercontent.com/NNlNJr0RD82aVJ873ePUvhQeLyzrMAutnZEtLBNQZhDT_4ez1HOgMzgPgfMUyo9I89vNmKVAGeFUWkRDymVsxHekhd8ftiTEZa30q5oWs8m9xpfK2vpU2u5jbLbZmCJYVavWp9i6Ih3u)

 *Figure 2 How to Distribute the Investment*

### Python Package

- GeoPandas & Pandas & Numpy

- Matplotlib & Seaborn

- scikit-learn

## Expected Outcomes

- Descriptive statistics and related map to show the distribution of different types of green investment. 

- Gentrification index and gentrified region map.

- Regression results to show the relationship between climate investment and green gentrification. 

## Bibliography

Hess, C. L. (2020). Light-Rail Investment in Seattle: Gentrification Pressures and Trends in Neighborhood Ethnoracial Composition. Urban Affairs Review, 56(1), 154–187. https://doi.org/10.1177/1078087418758959

Maantay, J., & Maroko, A. (2018). Brownfields to Greenfields: Environmental Justice Versus Environmental Gentrification. International Journal of Environmental Research and Public
Health, 15(10), 2233. https://doi.org/10.3390/ijerph15102233

Walker, R. H. (2021). Engineering gentrification: Urban redevelopment, sustainability policy, and green stormwater infrastructure in Minneapolis. Journal of Environmental Policy &
Planning, 23(5), 646–664. https://doi.org/10.1080/1523908X.2021.1945917

Benson, E. M., & Bereitschaft, B. (2020). Are LEED-ND developments catalysts of neighborhood gentrification? International Journal of Urban Sustainable Development, 12(1), 73–88. https://doi.org/10.1080/19463138.2019.1658588

Anderson, C. M., Kissel, K. A., Field, C. B., & Mach, K. J. (2018). Climate Change Mitigation, Air Pollution, and Environmental Justice in California. Environmental Science & Technology, 52(18), 10829–10838. https://doi.org/10.1021/acs.est.8b00908

Cushing, L., Blaustein-Rejto, D., Wander, M., Pastor, M., Sadd, J., Zhu, A., & Morello-Frosch, R. (2018). Carbon trading, co-pollutants, and environmental equity: Evidence from California’s cap-and-trade program (2011–2015). PLOS Medicine, 15(7), e1002604. https://doi.org/10.1371/journal.pmed.1002604

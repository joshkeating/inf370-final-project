# Project Proposal

## Project Description

The overarching goal of this project is to investigate the causes of suicide rates. We are primarily concerned with the rates within the United States but we hope to contextualize these rates within scope of global suicide measurements. This sensitive topic area is important enough that the WHO recently classified suicide as a [global mental health issue](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5454768/). Suicide is such a serious public health issue that it is the second leading cause of death among individuals aged 15 to 29 globally. Due to the severity of the phenomenon, suicide has been widely researched and there are various factors that are presumed to have an effect on global rates. These factors are many and wide ranging but there is no conclusive link between any of them and suicide. This is likely due to the complexity of mental health and the myriad of ways one’s mental health can be affected. Some studies in the past have expolored links between [depression](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3330161/), [sociaecominic factors](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5454768/),  overall [happiness indexes](https://www.researchgate.net/publication/228462399_Dark_Contrasts_The_Paradox_of_High_Rates_of_Suicide_in_Happy_Places) or rates of [antidepressent prescriptsions](https://ajp.psychiatryonline.org/doi/abs/10.1176/ajp.2006.163.11.1898). After conducting research into this domain it was clear to us that suicide rates could be impacted by these variables as well as a host of others. We were curious if by combining a number of these variables we could predict suicide rates with a level of reasonable accuracy. At this point we have hypothesized that a combination of depression rates, economic equality, diet, time, sunlight, and gun ownership affects the rate of suicide in the United States.  

We have currently identified two datasets that will help us answer our hypothesis. The first is aggregated suicide numbers from across the world compiled by the WHO. This dataset ranges from 1980-2017 and is split up by country, sex, and age. The second of our datasets is is state level data collected by the CDC. This dataset has deaths and rates for each state from 2005 to 2016. As we progress we plan to collect additional datasets for information on the factors we have identified that may impact suicide rates. In order to test our hypothesis we plan on using a multivariate regression (either polynomial or linear depending on investigation) and K-nearest neighbors (KNN) to help us predict suicide rates. Our target audience is anyone living in the US. This is because suicide is an issue that affects everyone, directly or indirectly. We hope that our audience gains a broader understanding of this important issue and the causes that contribute to it. 

## Technical Description

We plan to publish our findings in a static `HTML` page that is generated using `KnitR`. Our biggest challenge will be finding and joining auxiliary data to our original dataset. We will be investigating several socioeconomic factors that are not included in the primary dataset. To complete the project we will need to learn how to build data visualizations using python libraries. To conduct our analysis we will use the following approach:

- Create and attach additional features to our existing datasets
- Deal with null values using the appropriate technique for the data type and context in the dataset.
- Conduct a in depth exploratory analysis of all of our datasets.
- Normalize the data and test different polynomial transformations.
- Use grid search to determine the optimal parameters of our model.
- Run our regression using our selected features.

In taking on this project, we expect our biggest challenge to be locating and joining auxiliary feature datasets to our main aggregated one.

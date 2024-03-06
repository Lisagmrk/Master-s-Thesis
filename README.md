## The Effects of Economic Sanctions on Russia from 2014 to 2021

This code is part of my master's thesis in which I examine the impact of US and EU sanctions on Russia after its annexation of Crimea in 2014. It is a work in progress and will be updated regularly. The raw data is from the US Office of Foreign Assets Control [(OFAC)](https://ofac.treasury.gov/) and the Council of the European Union [(EU Council)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A02014D0145-20230915&qid=1703029680787). 

The **constructing_dataset** notebook cleans these officialy sanctions lists, divides them each into targeted individuals and targeted entities, and then merges them to a comprehensive list of sanctioned individuals and sanctioned entities. It then identifies firms that are not explicitly mentioned in the sanctions list, but are nevertheless sanctioned for one of the following reasons:
- Their Global Ultimate Owner (GUO) was sanctioned
- Their Majority Shareholder was sanctioned
- Their are a subsidiary of a sanctioned firm
  
Finally, the code matches the comprehensive dataset of all targeted entities with data on economic performance from the [ORBIS](https://www.bvdinfo.com/en-gb/) Europe dataset.

The **summary_statistics** notebook performs exploratory analysis to get an overview over the data.

The **analysis_1** notebook applies the Synthetic Control Method to estimate the causal effect of sanctions on Russia's GDP per capita (PPP). The findings suggest that the sanctions cost around 2000 US dollars in GDP per capita and that this negative effect persisted until the end of the observation period in 2021, although the magnitude of the effect decreased over time.

Below are the findings of this analysis, followed by some summary statistics.

### Synthetic Control Method: Effect of Sanctions on Russia's GDP per capita (PPP)

![Untitled](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/93657bbe-863a-4c8d-9a96-1fcb6b0e7139)


Placebo Tests

![Untitled](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/3cb405d8-a8cd-4980-88df-383f3dff735d)


### **Summary Statistics**
Sanctioned Firms across Industries

![Untitled](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/06a129af-59c8-4f78-bc8e-a2193fe79a5d)

![image](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/fb992822-a519-42f2-9c5d-2dd2a5683c06)

Sanctioned Firms by Sanctioning Government

![Untitled-1](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/7c8bcab7-4e38-47f5-9bb1-727a4ae005b4)

Total Number of Sanctioned Firms in 2014

![Untitled](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/1a7d826f-3a17-4a2f-af8c-5ba03d36d5ff)

Number of Sanctioned Firms by Type

![Untitled-1](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/8278d2f2-323c-4fab-a4ae-e93e9b63c5b0)





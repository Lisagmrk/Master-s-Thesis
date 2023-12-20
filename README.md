## US and EU Sanctions on Russia after 2014

This code is part of my master's thesis in which I examine the impact of US and EU sanctions on Russia after its annexation of Crimea in 2014. The raw data is from the US Office of Foreign Assets Control [(OFAC)](https://ofac.treasury.gov/) and the Council of the European Union [(EU Council)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A02014D0145-20230915&qid=1703029680787). The code cleans these officialy sanctions lists, divides them each into targeted individuals and targeted entities, and then merges them to a comprehensive list of sanctioned individuals and sanctioned entities. It then identifies firms that are not explicitly mentioned in the sanctions list, but are nevertheless sanctioned for one of the following reasons:
- Their Global Ultimate Owner (GUO) was sanctioned
- Their Majority Shareholder was sanctioned
- Their are a subsidiary of a sanctioned firm

Finally, the code matches the comprehensive dataset of all targeted entities with data on economic performance from the [ORBIS](https://www.bvdinfo.com/en-gb/) Europe dataset.

Below are some summary statistics of the of the final dataset.

![image](https://github.com/Lisagmrk/Masters-Thesis/assets/64646346/e97003c5-77fa-473d-81b5-1865191d15ca)


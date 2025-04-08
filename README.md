# DSA-210-Term-Project
Sabanci University 2025 Spring term DSA 210 Lecture term project

## **Project Idea**

This project investigates the evolving preferences of anime fans within the rapidly expanding global anime market. Once a niche interest, anime has achieved mainstream popularity, driven by its distinctive art styles and compelling narratives. The anime market, valued at USD 31.41 billion in 2023 and projected to reach USD 72.86 billion by 2032 (CAGR 9.8%), necessitates a deeper understanding of consumer trends. This research will analyze data from platforms like MyAnimeList and AniList, alongside with relevant economic and demographic data from sources like the IMF and World Bank, to identify key drivers of anime fan preferences. Specifically, this study will explore how factors such as genre. popularity, location, age, and gdp per capita correlate with user ratings and engagement.

## **Motivation**

There are currently over 10000 animes currently on the internet. Just the current Winter 2025 season had 165 anime. With over 10,000 anime available and new seasons introducing hundreds more, navigating the vast anime landscape is challenging for both new and long-time fans. To build an effective anime recommendation AI, we must first understand the key elements driving viewer preferences. This project will first find these key elements and secondly will create an anime recommendation AI using these key elements.

## **Sources of Data**

Main source will be the datasets I found in kaggle about anime. If possible data scrapping will be used to find more recent data.
Addition data like GDP per capita and etc. will be found from reliable international sources like World Bank

Dataset Links:
https://www.kaggle.com/datasets/azathoth42/myanimelist
https://www.kaggle.com/datasets/mathurinache/world-happiness-report/data
https://data.worldbank.org/indicator (extensive global metrics)

## **Description of the Dataset**

The dataset for this project consists of data from online resources. Here is what I will try to find and implement:

### **From kaggle - azathoth42/myanimelist** 
- **Gender**: The gender of the user
- **Birth Date**: The user's birth year
- **Join Date**: The year user joined
- **User Watching**: The amount of anime the user is currently watching
- **User Completed**: The amount of anime the user completed
- **User On Hold**: The amount of anime the user stopped watching
- **User Dropped**: The amount of anime the user dropped
- **User Plan to Watch**: The amount of anime the user is planning to watch
- **User Days Spent Watching**: The amount of days the user spent watching anime
- **User Location**: The location(country) of the user  
- **User Mean Score**: Mean score of the scores given by the user
- **User Watched Episodes**: Amount of episodes watched by the user
- **User Rewatched Episodes**: Amount of episodes rewatched by the user

### **From kaggle - mathurinache/world-happiness-report** 
- **Happiness Score**: The happiness score of the country from the happiness index

### **From World Bank**
- **Agricultural land (% of land area)**: Percentage of a country's land used for farming or agriculture
- **Forest area (% of land area)**: Percentage of land area covered by forests
- **Rural population (% of total population)**: Share of the total population living in rural areas
- **Agriculture, forestry, and fishing, value added (% of GDP)**: Share of agriculture, forestry, and fishing in the country's GDP
- **Maternal mortality ratio (modeled estimate, per 100,000 live births)**: Number of women who die during pregnancy or childbirth per 100,000 live births
- **Income share held by lowest 20%**: Share of income held by the poorest 20% of the population
- **Income share held by highest 20%**: Share of income held by the richest 20% of the population
- **Mortality rate, under-5 (per 1,000 live births)**: Number of children under age 5 who die per 1,000 live births
- **Net migration**: Difference between the number of people entering and leaving a country
- **Poverty headcount ratio at $2.15 a day (2017 PPP) (% of population)**: Percentage of people living on less than $2.15 per day
- **Access to electricity (% of population)**: Percentage of the population with access to electricity
- **Electric power consumption (kWh per capita)**: Average electricity consumed per person per year
- **CPIA public sector management and institutions cluster average (1=low to 6=high)**: Rating of how effective and accountable a country's public sector is (1–6 scale)
- **Population growth (annual %)**: Annual growth rate of the total population
- **Renewable electricity output (% of total electricity output)**: Percentage of electricity generated from renewable sources
- **Urban population (% of total population)**: Share of people living in urban areas
- **Central government debt, total (% of GDP)**: Public debt as a percentage of GDP
- **GDP per capita (current US$)**: Average income per person in the country
- **GDP per capita growth (annual %)**: How fast GDP per person is increasing annually
- **GNI per capita, PPP (current international $)**: Average income per person, adjusted for cost of living
- **Inflation, consumer prices (annual %)**: Yearly increase in consumer prices
- **Government expenditure on education, total (% of GDP)**: Government spending on education as a percentage of GDP
- **Literacy rate, adult total (% of people ages 15 and above)**: Percentage of adults (15+) who can read and write
- **Literacy rate, youth total (% of people ages 15-24)**: Percentage of young people (15–24) who can read and write
- **Time required to get electricity (days)**: Average time (in days) to get a new electricity connection
- **Renewable internal freshwater resources per capita (cubic meters)**: Average renewable water available per person per year
- **Strength of legal rights index (0=weak to 12=strong)**: Score indicating how strong legal protections are for borrowers and lenders (0–12)
- **Firms with female participation in ownership (% of firms)**: Percentage of businesses with at least one woman owner
- **Labor force, female (% of total labor force)**: Percentage of the workforce that is female
- **Contraceptive prevalence, any method (% of married women ages 15-49)**: Share of married women using any contraception
- **Life expectancy at birth, female (years)**: Average lifespan of women
- **Life expectancy at birth, male (years)**: Average lifespan of men
- **Teenage mothers (% of women ages 15-19 who have had children or are currently pregnant)**: Percentage of teenage girls (15–19) who are mothers or pregnant
- **Fertility rate, total (births per woman)**: Average number of children born per woman
- **Cause of death, by injury (% of total)**: Share of deaths caused by injuries
- **Death rate, crude (per 1,000 people)**: Number of deaths per 1,000 people per year
- **Fixed broadband subscriptions (per 100 people)**: Fixed broadband subscriptions per 100 people
- **Mobile cellular subscriptions (per 100 people)**: Mobile phone subscriptions per 100 people
- **Secure Internet servers (per 1 million people)**: Number of secure servers per million people
- **High-technology exports (current US$)**: Total value of high-tech goods exported
- **Logistics performance index Overall (1=low to 5=high)**: Score measuring efficiency of trade and transport infrastructure (1–5 scale)
- **Medium and high-tech exports (% manufactured exports)**: Share of manufactured exports that are tech-intensive
- **New businesses registered (number)**: Number of new companies registered in a year
- **Population, total**: Number of people living in the country
- **Military expenditure (% of GDP)**: Military expenditure as a percentage of GDP
- **Tax revenue (% of GDP)**: Government tax revenue as a percentage of GDP
- **Unemployment, total (% of total labor force) (modeled ILO estimate)**: Percentage of the labor force that is unemployed
- **Employment to population ratio, 15+, total (%) (modeled ILO estimate)**: Percentage of adults (15+) who are employed
- **Exports of goods and services (% of GDP)**: Value of exported goods/services as a percentage of GDP
- **PM2.5 air pollution, mean annual exposure (micrograms per cubic meter)**: Average exposure to fine air particles (PM2.5) in µg/m³
- **Population density (people per sq. km of land area)**: Number of people per square kilometer of land
- **Population in the largest city (% of urban population)**: Share of urban population living in the biggest city
- **Population in urban agglomerations of more than 1 million (% of total population)**: Share of total population in very large urban areas (1M+ population)
- **School enrollment, primary and secondary (gross), gender parity index (GPI)**: Ratio of girls to boys enrolled in primary and secondary school
- **Refugee population by country or territory of asylum**: Number of refugees hosted by the country

## **Conclusion**

By the end of this project, I hope to answer the following questions:

- Which factors most influence an anime's popularity?  
- Can wwe guess how succesfull an anime is going to be before airing?  
- Are myths like romance is more popular among females and action is more popular among males realy true??  
- Can we apply these insights to create an anime recommendation AI?

# Luxury in Lockdown: What can the Covid-19 pandemic teach us about the behaviour of luxury goods in economic downturns and the lipstick index as an economic indicator?

## Overview 
The "Luxury in Lockdown" project investigates changes in the luxury goods market during the Covid-19 pandemic, with a specific focus on why the "lipstick index" did not hold during this period. Over the past century, during all economic downturns, an increase in revenue for lipstick has been recorded. The theory behind this is that consumers turn to affordable luxury rather than big ticket luxury items, such as holidays and fancy cars, when the economy is not doing as well. The analysis involves looking at changes in the luxury goods market overall, a zoom-in on what happened for cosmetics and analysis of why the above occurred focussing on ecommerce and mask mandates. This project highlights the different effect of a global health crisis and the consequent economic downturn on the luxury market, particularly cosmetics, compared to previous financial crises. 

## Objectives
• Understanding of what happened across the luxury market during the pandemic.\
• Understanding the alteration of the lipstick index towards the eyes. \
• Understanding which factors were most influential for revenue in luxury cosmetics.\
• The role of e-commerce in luxury good consumption. \
• The role of mask mandates on consumer behaviour. 

## Blog post link 
https://hackmd.io/@oYKGWySaT12DWp8R_EdiBQ/SJwfyzYJgl

## Project structure 
The repository contains everything you need to recreate the visualisations from my blog. 
### Folder structure

```
luxury_goods_project/
├── data/
│   ├── country_data/
│   │   ├── China/
│   │   │   ├── china_cci.csv
│   │   │   ├── china_eyes_onoff.csv
│   │   │   ├── china_face_onoff.csv
│   │   │   ├── china_lips_onoff.csv
│   │   │   ├── china_revenue.csv
│   │   │   └── china_unemployment.csv
│   │   ├── Germany/
│   │   │   ├── germany_cci.csv
│   │   │   ├── germany_eyes_onoff.csv
│   │   │   ├── germany_face_onoff.csv
│   │   │   ├── germany_lips_onoff.csv
│   │   │   ├── germany_revenue.csv
│   │   │   └── germany_unemployment.csv
│   │   ├── Japan/
│   │   │   ├── japan_cci.csv
│   │   │   ├── japan_eyes_onoff.csv
│   │   │   ├── japan_face_onoff.csv
│   │   │   ├── japan_lips_onoff.csv
│   │   │   ├── japan_revenue.csv
│   │   │   └── japan_unemployment.csv
│   │   ├── UK/
│   │   │   ├── uk_cci.csv
│   │   │   ├── uk_eyes_onoff.csv
│   │   │   ├── uk_face_onoff.csv
│   │   │   ├── uk_lips_onoff.csv
│   │   │   ├── uk_revenue.csv
│   │   │   └── uk_unemployment.csv
│   │   └── US/
│   │       ├── US_unemployment_rate.csv
│   │       ├── US_cos_frag_skin.csv
│   │       ├── segmented_luxcos_revenue.csv
│   │       ├── male_female_pop_ratio.csv
│   │       ├── lux_goods_US_revenue.csv
│   │       ├── Global_GDP.csv
│   │       ├── cosmetic_revenue_US.csv
│   │       ├── consumer_sentiment_US.csv
│   │       └── ecommerce/
│   │           ├── cosmetics_online_offline.csv
│   │           ├── eyes_ecommerce.csv
│   │           ├── face_ecommerce.csv
│   │           ├── lips_online_sales.csv
│   │           ├── lux_cosmetics_US_online_offline.csv
│   │           ├── lux_fashion_online_offline_USA.csv
│   │           ├── lux_goods_ecommerce_revenue.csv
│   │           ├── lux_leather_online_offline.csv
│   │           └── online_offline_USA.csv
│   └── excel_datasets/ (not used)
│
├── figures/
│   ├── causal_forest_notused.png
│   ├── cosmetic_revenue_indexed_graph.png
│   ├── feature_importance_graph.png
│   ├── luxcos_segmented_graph.png
│   ├── luxury_revenue_graph.png
│   ├── mask_population_pie.png
│   ├── online_sales_shares_graph.png
│   └── USA_map_plot.png
│
├── cr.md
├── dataset_sources.pdf
├── README.md
├── blog.txt
├── visualisations_code.pdf
└── visualisations_code.ipynb
```
### What are the documents included in the luxury_goods_project folder
**data** - includes all the csv files used in the analysis and some excel spreadsheets which have been converted into csvs.

**figures** - includes png files for all the visualisations created.

**cr.md** - created to allow github to track changes and the creation of the blog on hackMD.

**dataset_sources.pdf** - pdf of showing the source of every csv file in the "data" folder.

**README.md** - this document.

**blog.txt** - includes the link to my finished blog post on hackMD and the link to my Github repository.

**visualisations_code.pdf** - the pdf version of the output of my code on my machine.

**visualisations_code.ipynb** - Visualisations_code includes all the data cleaning, dataframe creation and visualisation creation steps. It is structured as follows: 

### Title: Code for Visualisations in Blog

#### 1. Install Packages and Change Working Directory 

#### 2. Visualisations

##### 2.1 Macro Perspective of Luxury Goods During Covid for the USA
- **2.1.1** Create Luxury Goods Dataframe and Clean Data for Graph
- **2.1.2** Code Visualisation for Luxury Goods Before, During, and After Covid-19

##### 2.2 Cosmetics and the Lipstick Index During Covid in the USA
- **2.2.1** Create Luxury Cosmetic Dataframe Separated by Category and Clean
- **2.2.2** Create Line Graph for Prestige Eyes, Lips, and Face Over Time
- **2.2.3** Dataframe and Clean for Prestige Cosmetics and Overall US Cosmetics
- **2.2.4** Indexed Graph for Prestige Cosmetics and Cosmetics Market Overall

#### 3. Advanced Modelling Analysis

##### 3.1 Data Cleaning for the USA
- **3.1.1** USA Revenue Column
- **3.1.2** USA GDP Column
- **3.1.3** Consumer Confidence USA Column
- **3.1.4** Unemployment Rate in USA Column
- **3.1.5** E-commerce Cosmetic Product USA Column
- **3.1.6** Create USA Dataframe

##### 3.2 Data Cleaning for Other Countries (China, Germany, Japan, and UK)
- **3.2.1** China
- **3.2.2** Germany
- **3.2.3** Japan
- **3.2.4** UK

##### 3.3 Large Dataframe (All Countries Combined and Cleaned)

##### 3.4 Causal Forest Analysis

##### 3.5 Random Forest Model

##### 3.6 Correlation Between GDP Change and Revenue of the Cosmetic Industry

#### 4. Further Visualisations Building on Advanced Models

##### 4.1 E-commerce
- **4.1.1** Dataframes and Data Cleaning
- **4.1.2** Online Sales Plot

##### 4.2 Mask Mandates
- **4.2.1** Mask Mandates Across the USA Length Data Cleaning
- **4.2.2** Mask Mandates Choropleth Map
- **4.2.3** Mask Mandate Proportion of Population Data Cleaning

If you are only interested in the visualisations run all the code and close the cleaning sections where necessary.

If you are only interested in the cleaning parts run all the code and close the Plots and Map sections where necessary.

## How to run the code on your machine

### Step 1
Download the folder named "730022777" and take the "luxury_goods_project" folder OUT of it. Save this to your computer. 

### Step 2 
Open the whole "luxury_goods_project" folder on VScode. All the files and folders within the "luxury_goods_project" should now be listed on left-hand side of the screen. You can use other platforms to open the code, however, given the code uses lots of csv files, it is easier to replicate using vscode.

### Step 3 
Next, open "visualisations_code.ipynb"

### Step 4 
Run the first line of code in section 1 "1. Install packages and change working directory". It is extremely important that this code WORKS and all packages are installed. If they are not installed, use pip install in your terminal. 

### Step 5 
Alter the working directory in block 2 (directly underneath the code from step 4). This is also extremely important. Currently, it is set for my laptop. To do this, you need to copy the pathname from where you saved the "luxury_goods_project" folder on your laptop into where it says "/Users/kaitlinjohnson/Desktop/luxury_goods_project". Only paste up to and including "luxury_goods_project".

### Step 6 
You should be good to go and run all the code blocks. 


## Requirements 
1. Pandas
2. Matplotlib.pyplot
3. seaborn
4. numpy
5. os
6. plotly.express
7. econml.dml
8. sklearn.ensemble
9. sklearn.model_selection
10. sklearn.preprocessing
11. random
12. sklearn.metrics

## Notes 
- Excel files, causal forest analysis and the causal_forest_notused.png are included in the project folder but NOT used directly. These files are included for completeness but are not used in the main analysis.

# Ameyaa-Desai-Personal-Dataset-Project
This is the repository for my personal dataset project

# Background
Each year, Pinterest releases its [“Pinterest Palette”](https://business.pinterest.com/blog/2025-pinterest-palette-this-years-trending-colors/), a collection of five colors they believe will shape design, fashion, and cultural aesthetics in the coming year. These selections stem from Pinterest’s proprietary trend-spotting methodology, which draws on years of data-driven forecasting through Pinterest Predicts. In this project, I examine how these predicted colors actually play out beyond the Pinterest ecosystem. While Pinterest identifies five potential “colors of the year,” my goal is to determine which color truly resonates most with the broader public. To do this, I take Pinterest’s chosen palette and compare the five colors using Google Trends data, analyzing search interest to identify which color captured the most attention.

# Motivating Question
Can the Pinterest Palette be trusted by businesses hoping to capitalize on emerging aesthetics, and which of its predicted colors ultimately proved most popular over the year?

# Data
I selected Google Trends as the primary data source because it offers a reliable, real-time measure of public interest across a broad and diverse user base. While Pinterest’s palette predictions originate within its own platform ecosystem, Google Trends reflects search behavior from the general population, making it an ideal tool for testing whether Pinterest’s anticipated colors actually resonate beyond its own users. Google is the most widely used search engine in the world, so fluctuations in search volume provide a strong indicator of how much attention each color attracts in everyday online behavior. By comparing Pinterest’s curated predictions to Google Trends’ real-world search data, I am able to evaluate the palette’s predictive accuracy and determine which colors captured genuine public interest over the year. I collected the data of how many searches each of Pintrest's five colors (butter yellow, dill green, indigo aura, cherry red, and alpine oat) had over the course this year. 

# Data Cleaning
I started by making sure all the data sets I collected through Google Trends only represented the year of 2025. Then, I changed the Week column from showing the numerical dates (e.g. 01-06-25) to just Week 1. I also made sure that the column headers were "Week" and "Searches" for each dataset. 

# Line Plot of Weekly Search Interest
![Color Trends Line Plot] (https://github.com/ameyaadesai/Ameyaa-Desai-Personal-Dataset-Project/blob/a2d143032fe55c170ed53dbc326c057dd56fc9a7/colortrendsline.png)

The first graph I created was a line plot comparing weekly Google Trends search interest for all five colors in the Pinterest Palette. I chose this graph because it gave me the most direct way to visualize how each color’s popularity changed over time, which aligns with my goal of understanding whether Pinterest’s predictions actually match broader public attention. From this visualization, I immediately learned that Cherry Red and Indigo Aura consistently showed higher search interest than the other colors, with Cherry Red especially standing out across most weeks. Butter Yellow stayed in the mid-range, showing modest but steady interest, while Dill Green and Alpine Oat rarely rose above the bottom, often staying close to zero.

Based on this graph alone, Cherry Red appeared to be the strongest contender for the year’s true “color of the year,” followed closely by Indigo Aura. The line plot revealed that not all Pinterest-predicted colors gained meaningful traction, and that some colors resonated far more with the public than others. However, because the lines overlapped often, the graph was visually dense, which pushed me to explore clearer comparison methods in the next visualization.


## Google Trends Search Interest for 2025 Color of the Year

![Color Trends Plot](https://github.com/ameyaadesai/Ameyaa-Desai-Personal-Dataset-Project/blob/main/color_trends_plot.png?raw=true)


This plot compares Google Trends weekly search interest for Butter Yellow and Dill Green—two colors predicted as potential “Color of the Year” candidates for 2025. Butter Yellow shows a strong rise through mid-year with peak interest around weeks 25–30 before gradually declining, whereas Dill Green exhibits more variable and generally lower search volumes. The higher and more sustained interest in Butter Yellow suggests that public attention leaned more heavily toward this color during the year.

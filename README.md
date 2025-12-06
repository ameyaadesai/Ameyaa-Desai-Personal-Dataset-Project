# Ameyaa-Desai-Personal-Dataset-Project

# Background
Each year, Pinterest releases its [“Pinterest Palette”](https://business.pinterest.com/blog/2025-pinterest-palette-this-years-trending-colors/), a collection of five colors they believe will shape design, fashion, and cultural aesthetics in the coming year. These selections stem from Pinterest’s proprietary trend-spotting methodology, which draws on years of data-driven forecasting through Pinterest Predicts. In this project, I examine how these predicted colors actually play out beyond the Pinterest ecosystem. While Pinterest identifies five potential “colors of the year,” my goal is to determine which color truly resonates most with the broader public. To do this, I take Pinterest’s chosen palette and compare the five colors using Google Trends data, analyzing search interest to identify which color captured the most attention.

# Motivating Question
Can the Pinterest Palette be trusted by businesses hoping to capitalize on emerging aesthetics, and which of its predicted colors ultimately proved most popular over the year?

# Data
I selected Google Trends as the primary data source because it offers a reliable, real-time measure of public interest across a broad and diverse user base. While Pinterest’s palette predictions originate within its own platform ecosystem, Google Trends reflects search behavior from the general population, making it an ideal tool for testing whether Pinterest’s anticipated colors actually resonate beyond its own users. Google is the most widely used search engine in the world, so fluctuations in search volume provide a strong indicator of how much attention each color attracts in everyday online behavior. By comparing Pinterest’s curated predictions to Google Trends’ real-world search data, I am able to evaluate the palette’s predictive accuracy and determine which colors captured genuine public interest over the year. I collected the data of how many searches each of Pintrest's five colors (butter yellow, dill green, indigo aura, cherry red, and alpine oat) had over the course this year. 

# Data Cleaning
To begin the analysis, I first standardized all of the datasets that I collected from Google Trends so that they only reflected search activity from the year 2025. Google Trends exports dates in a month–day–year format (for example, “01-06-25”), so my next step was to convert these dates into a simple sequential Week variable. This created a unified timeline across all five color datasets. This was important because the original date format differed slightly between the downloaded files, and converting them into week numbers ensured that all of the colors could be compared on the exact same scale and aligned properly when visualizing trends.

I also went through each dataset to ensure consistent column naming. Specifically, I standardized the column headers to “Week” and “Searches” across all five color files. Google Trends sometimes labels the second column as “Interest” or adds extra spaces depending on how the file is exported, so cleaning these names prevented errors later when merging files, applying functions, or mapping variables during plotting. 

# Line Plot of Weekly Search Interest
![Color Trends Line Plot](https://github.com/ameyaadesai/Ameyaa-Desai-Personal-Dataset-Project/blob/a2d143032fe55c170ed53dbc326c057dd56fc9a7/colortrendsline.png)

The first graph I created was a line plot comparing weekly Google Trends search interest for all five colors in the Pinterest Palette. I chose this graph because it gave me the most direct way to visualize how each color’s popularity changed over time, which aligns with my goal of understanding whether Pinterest’s predictions actually match broader public attention. From this visualization, I immediately learned that Cherry Red and Indigo Aura consistently showed higher search interest than the other colors, with Cherry Red especially standing out across most weeks. Butter Yellow stayed in the mid-range, showing modest but steady interest, while Dill Green and Alpine Oat rarely rose above the bottom, often staying close to zero.

Based on this graph alone, Cherry Red appeared to be the strongest contender for the year’s true “color of the year,” followed closely by Indigo Aura. The line plot revealed that not all Pinterest-predicted colors gained meaningful traction, and that some colors resonated far more with the public than others. However, because the lines overlapped often, the graph was visually dense, which pushed me to explore clearer comparison methods in the next visualization.


# Boxplots of Search Interest Distributions
![Color Trends Boxplots](https://github.com/ameyaadesai/Ameyaa-Desai-Personal-Dataset-Project/blob/8cff036ed63b8e9f3c6a88ef441361df4b16f14c/colortrends_boxplot.png)

After noticing how cluttered the line plot was, I created boxplots to compare the distribution of search interest for each color throughout the year. This visualization helped me summarize the overall performance of each color without focusing on the week-to-week noise. When I examined the boxplots, I was surprised to see that Butter Yellow actually performed much better than Indigo Aura in terms of distribution. Butter Yellow had a much higher median, as well as a tighter spread of consistently mid-to-high values.

In contrast, Indigo Aura’s boxplot revealed a lot of low or zero values, indicating that although it had a strong spike at some point, it wasn’t consistently popular overall. Cherry Red still had the strongest distribution, with high central values and surprisingly stable interest across the year. Meanwhile, Dill Green and Alpine Oat showed extremely low medians and large spreads, confirming that they were the weakest performers.

From this visualization, I learned that Butter Yellow was actually a stronger overall contender than Indigo Aura when looking at year-long popularity. This challenged my initial assumptions from the line plot and showed me the value of analyzing the data from multiple angles.

# Dot Plot Showing Weekly Rank Positions
![Color Trends Dot Plot](https://github.com/ameyaadesai/Ameyaa-Desai-Personal-Dataset-Project/blob/8cff036ed63b8e9f3c6a88ef441361df4b16f14c/colortrends_dotplot.png)

For my final graph, I transformed the weekly search values into ranks and visualized them using a dot plot. I chose this graph because it directly answers my motivating question: which color was truly the most popular throughout the year? Rather than comparing raw numbers, ranking each color weekly allowed me to see exactly who “won” each week and whether Pinterest’s predictions aligned with actual public interest. The first two visualizations showed overall trends and distributions, but they didn’t directly answer the question of which color actually dominated the most weeks, which is essential to my goal of evaluating Pinterest’s predictions.

When I examined the graph, one of the first things I noticed was just how consistently Butter Yellow occupied Rank 1. This was especially interesting because earlier graphs suggested that Cherry Red had higher peaks and a stronger overall average. However, the dot plot revealed that Cherry Red’s popularity was more variable. It spent many weeks in Rank 2 or Rank 3, even if its high points were very high. In contrast, Butter Yellow maintained steady search interest that kept it consistently competitive and frequently on top. The plot also highlighted how Indigo Aura’s popularity was uneven. It appeared in Rank 1 or Rank 2 during a few isolated weeks, but it also dropped to lower ranks often, reflecting the many weeks where its search values were at or near zero. Meanwhile, Dill Green and Alpine Oat remained near the bottom for most of the year, reinforcing their lack of traction compared to the other colors in the palette.


# Conclusion
Through analyzing Google Trends data with line plots, boxplots, and weekly rank comparisons, I found that the Pinterest Palette offers some useful guidance, but not all of its predicted colors gained strong public attention. While Cherry Red showed the highest peaks in search interest, the broader patterns revealed something more surprising: Butter Yellow was actually the most consistently popular color throughout 2025. The boxplots showed that it had a higher and more stable distribution than most other colors, and the weekly rank dot plot confirmed that Butter Yellow held the top position more weeks than any other shade.

Indigo Aura showed occasional spikes but lacked consistency, and Alpine Oat and Dill Green rarely appeared near the top at all. This suggests that Pinterest correctly predicted some important colors, but businesses should still look at real-world data to understand how interest evolves over time. Overall, Pinterest’s palette is partially reliable, and based on my analysis, Butter Yellow emerges as the true top-performing color of the year.


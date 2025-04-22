# Exploratory Data Analysis of the 2024 Summer Olympics Medal Table Using Power Query in Excel
## 📘 1. Introduction
The 2024 Summer Olympics, held in Paris, France, brought together athletes from all over the world to compete in a wide array of sports. This analysis aims to explore the distribution of medals among participating countries, identify top performers, and uncover interesting patterns in the medal table. We will analyze the medal counts — gold, silver, bronze, and total — for each country and use visualizations to enhance our understanding of performance trends.

## 🧩 2. Data Extraction and Preparation (ETL Process)
Before beginning the analysis, I performed an **ETL (Extract, Transform, Load)** process using **Power Query** in **Microsoft Excel**:

**Extract:** Data was sourced directly from the official [Wikipedia medal table](https://en.wikipedia.org/wiki/2024_Summer_Olympics_medal_table).

**Transform:** Unnecessary rows and columns were removed, column names were cleaned, and data types were verified to ensure consistency.

**Load:** The cleaned dataset was loaded into Excel for further analysis.

### 🔄 Why Power Query?
Power Query enables **automatic data refresh**. While Olympic medal data is generally static after the event concludes, if any updates or corrections are made on the Wikipedia page, Power Query allows the Excel sheet to reflect those changes instantly upon refresh. This makes the dataset both dynamic and maintainable for any future updates.

This streamlined **ETL process** ensured that the data was accurate, well-structured, and ready for in-depth analysis using Excel tools such as pivot tables, charts, and summary statistics.

## 📊 3. Dataset Overview
The dataset includes the following fields for each country:

* Rank: Overall rank based on medal count
* Country: Nation or National Olympic Committee (NOC)
* Gold: Count of gold medals won
* Silver: Count of silver medals won
* Bronze: Count of bronze medals won
* Total: Total number of medals won

## 📈 4. Descriptive Statistics

| Metric                          | Value  |
|----------------------------------|--------|
| 🏳️ Total Countries               | 92     |
| 🥇 Total Gold Medals             | 329    |
| 🥈 Total Silver Medals           | 330    |
| 🥉 Total Bronze Medals           | 385    |
| 🎖️ Total Medals Awarded         | 1,044  |
| 🏆 Max Total Medals by a Country | 126    |
| 📈 Mean Total Medals             | 11.35  |
| 📉 Median Total Medals           | 5.0    |

## 🥇 5. Top Medal-Winning Countries

Top 10 Countries by Total Medals:

| Rank | Country           | Gold | Silver | Bronze | Total |
|------|-------------------|------|--------|--------|-------|
| 1    | United States     | 40   | 44     | 42     | 126   |
| 2    | China             | 40   | 27     | 24     | 91    |
| 3    | France* (Host)    | 16   | 26     | 22     | 64    |
| 4    | Australia         | 18   | 19     | 16     | 53    |
| 5    | Japan             | 20   | 12     | 13     | 45    |
| 6    | Great Britain     | 14   | 18     | 20     | 52    |
| 7    | Germany           | 13   | 12     | 10     | 35    |
| 8    | South Korea       | 12   | 11     | 13     | 36    |
| 9    | Italy             | 10   | 13     | 15     | 38    |
| 10   | Netherlands       | 8    | 9      | 8      | 25    |

## 📊 6. Charts and Visualizations
### 🔹 1. Clustered Bar Chart: Top 10 Countries by Total Medals
This chart displays the top 10 countries with the highest total medal counts. Each bar represents a country, with the length corresponding to the total number of medals won. It helps quickly identify the most successful nations overall.
![image](https://github.com/user-attachments/assets/b9501538-41e8-447a-b763-91e29ddfb9de)

### 🔹 2. Stacked Bar Chart: Top 10 Countries by Medal Type
This visualization breaks down each of the top 10 countries' total medals into gold, silver, and bronze. It helps highlight not only total performance but also how each country performed across different medal types.
![image](https://github.com/user-attachments/assets/db777bc8-cd9d-43a4-8b11-48b4ac6ef764)

### 🔹 3. Pie Chart: Top 10 Countries’ Share of Total Medals
This chart shows the percentage of total medals won by the top 10 countries. It gives a clear view of how medals are distributed among the leading nations and highlights any dominance or balance in the competition.
![image](https://github.com/user-attachments/assets/10953333-97c4-45e5-b8a5-a82c0664a2c4)

### 🔹 4. Treemap: Gold Medal Distribution – Top 10 Countries vs. Others
This Treemap highlights the distribution of gold medals among the top 10 countries, with all other countries grouped under a single “Others” category. Each block represents a country (or the Others group), and its size reflects the number of gold medals won. This visualization emphasizes which nations led in terms of top podium finishes, making it easy to spot gold medal dominance at a glance.
![image](https://github.com/user-attachments/assets/df78d46f-7679-4bfc-a54f-5c9244f1f3f7)

### 🔹 5. Scatter Plot: Gold Medals vs. Total Medals
This scatter plot displays the relationship between the number of gold medals and the total medals won by each country. Each point represents a country, where the x-axis shows gold medals and the y-axis shows total medals. The plot helps identify trends, such as whether countries winning more gold tend to perform better overall — and also highlights any outliers (e.g., countries with high totals but fewer golds).
![image](https://github.com/user-attachments/assets/fa49e734-7ddd-4ca0-a924-f45dc5625f53)

## ✅ 7. Conclusion
Using Power Query not only streamlined the ETL process but also ensured that any future updates from the source webpage would automatically reflect in the Excel file, offering a sustainable and dynamic approach to data analysis.

This Exploratory Data Analysis provided valuable insights into the distribution of medals at the 2024 Summer Olympics. Key observations include:

* The United States and China are clear leaders in both gold and total medals.

* France, the host country, performed strongly across all medal types.

* Medal distribution is heavily skewed toward a small group of high-performing countries.

* A strong correlation exists between gold medals and total medals, indicating that countries dominating gold also tend to perform well overall.



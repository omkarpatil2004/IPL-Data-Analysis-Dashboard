## 🏏 IPL Analysis Dashboard (Power BI)

### 📊 Project Overview

This Power BI project provides an **interactive and insightful analysis of the Indian Premier League (IPL)**.
It focuses on team and player performances, venue-based outcomes, toss impacts, and season-level statistics.
The dashboard helps cricket enthusiasts, analysts, and decision-makers uncover hidden trends and data-driven insights from IPL seasons.

---

### 🎯 Objective

The main goal of this project is to **analyze IPL data** using Power BI and derive meaningful insights, such as:

* Team performance comparison
* Top batsmen and bowlers of the season
* Venue-wise match results
* Toss decision impact on match outcomes
* Overall tournament statistics (sixes, fours, etc.)

---

### 🧠 Key Insights from the Dashboard (Sample: IPL 2021)

* 🏆 **Title Winner:** *Chennai Super Kings*
* 🟧 **Orange Cap (Most Runs):** *Ruturaj Gaikwad – 635 Runs*
* 🟪 **Purple Cap (Most Wickets):** *Harshal Patel – 32 Wickets*
* 💥 **Total Sixes:** 687
* 💥 **Total Fours:** 1550
* 📍 **Most Wins Venue:** Dubai International Stadium (9 Wins)
* 🪙 **Toss Decision Trend:** Teams winning the toss preferred batting (80%)

---

### 📈 Dashboard Features

#### 🏅 **Title & Player Stats**

* Displays tournament **winner**, **Orange Cap**, and **Purple Cap** holders.
* Shows the **total number of sixes and fours** hit during the season.

#### ⚾ **Batting Analysis**

* Dropdown filter to select any **batsman**.
* Displays:

  * Total Runs
  * 4s and 6s
  * Strike Rate

#### 🎯 **Bowling Analysis**

* Dropdown filter to select any **bowler**.
* Displays:

  * Wickets Taken
  * Economy Rate
  * Bowling Average
  * Bowling Strike Rate

#### 🏟️ **Venue Analysis**

* Bar chart showing **matches won by venue**, classified by:

  * Wins by Runs
  * Wins by Wickets
  * Wins by Super Over

#### 🧾 **Team Performance**

* Horizontal bar chart showing **total wins by each team** in the season.

#### 🪙 **Toss Impact Analysis**

* Pie charts showing:

  * Toss decisions (Bat/Field)
  * Match results based on toss outcome

---

### 🗂️ Dataset Details

The dataset used contains IPL data from various seasons (2008–2021).
It includes the following fields:

| Category                    | Columns                                                       |
| --------------------------- | ------------------------------------------------------------- |
| **Match Info**              | Season, Match ID, Date, Venue, Umpires                        |
| **Teams**                   | Team1, Team2, Winner, Toss Winner                             |
| **Toss Details**            | Toss Decision (Bat/Field), Result                             |
| **Player Stats**            | Player of Match, Orange Cap, Purple Cap                       |
| **Batting & Bowling Stats** | Runs, Fours, Sixes, Strike Rate, Wickets, Economy, Bowling SR |

📁 **Data Source:** Publicly available IPL datasets (Kaggle / official IPL stats)

---

### ⚙️ Tools & Technologies Used

* **Power BI Desktop** – Data modeling, transformation & visualization
* **Power Query Editor** – Data cleaning and preprocessing
* **DAX (Data Analysis Expressions)** – Custom calculations and KPIs
* **Excel / CSV Files** – Dataset storage format

---

### 🧩 Key DAX Measures Used

```DAX
Total Runs = SUM(Batting[Runs])
Total Fours = SUM(Batting[Fours])
Total Sixes = SUM(Batting[Sixes])
Strike Rate = DIVIDE(SUM(Batting[Runs]) * 100, SUM(Batting[Balls]))

Total Wickets = SUM(Bowling[Wickets])
Economy = DIVIDE(SUM(Bowling[Runs]), SUM(Bowling[Overs]))
Bowling Average = DIVIDE(SUM(Bowling[Runs]), SUM(Bowling[Wickets]))
Bowling SR = DIVIDE(SUM(Bowling[Balls]), SUM(Bowling[Wickets]))
```

---

### 🧹 Data Cleaning Steps

1. Removed duplicate records and null values.
2. Standardized team names and venue names.
3. Merged multiple tables (Matches, Players, Venues).
4. Created relationships between datasets for seamless interactivity.
5. Added calculated columns and measures using DAX.

---

### 📊 Visualizations Used

| Visualization Type | Description                                            |
| ------------------ | ------------------------------------------------------ |
| **Cards**          | Tournament highlights (Title Winner, Orange Cap, etc.) |
| **Bar Charts**     | Total wins by team, venue-wise wins                    |
| **Pie Charts**     | Toss decision analysis                                 |
| **Slicers**        | Season, Batsman, Bowler filters                        |
| **KPIs**           | Runs, Wickets, Strike Rate, Economy                    |

---

### 💡 Insights Derived

* Toss decisions significantly influence match outcomes.
* Certain venues consistently favor teams batting first.
* Top-performing players contribute heavily to team wins.
* Chennai Super Kings showed dominant performance in 2021.

---

### 🚀 How to Use

1. Download the `.pbix` file from this repository.
2. Open it in **Power BI Desktop**.
3. Explore different visuals using slicers and filters (Season, Player, Team, etc.).
4. Optionally, connect new IPL datasets (CSV/Excel) to update for other seasons.

---

### 📸 Dashboard Preview

![IPL Dashboard Preview](e029492f-688e-49e1-9b6c-6472269cbad6.png)

---

### 📁 Repository Structure

```
📦 IPL-Analysis-Dashboard
│
├── 📊 IPL_Analysis.pbix                # Power BI Project File
├── 📄 README.md                        # Project Documentation
├── 📂 dataset/
│   ├── matches.csv
│   ├── deliveries.csv
│   └── players.csv
└── 📸 dashboard_preview.png            # Dashboard Image
```

---

### 🧑‍💻 Author

**Omkar Abhaykumar Patil**
🎓 B.Tech – Computer Science and Business Systems
📊 Data Analytics | Power BI | Machine Learning Enthusiast

---

### 🏁 Conclusion

This IPL Analysis Power BI Dashboard provides **a complete data-driven overview of the tournament**, enabling users to explore, compare, and analyze performances at various levels — team, player, and venue.
It’s a perfect blend of **data storytelling and visual analytics** in sports data.


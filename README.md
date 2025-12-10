# Cricket-analysis

This project analyzes cricket batting performance across IPL, ODI, and T20 formats using a 50-record dataset containing real players.
The goal is to identify:

Players with strong average runs

Players with high strike rate (scoring efficiency)

Venue-wise batting performance trends

The final output is a Power BI dashboard with three key visuals.

🗂️ Dataset

Format: 50 records (Mixed IPL/ODI/T20)

Contains: Player name, runs, strike rate, balls, fours, sixes, venue, opposition, date

Source: Custom dataset generated for analytics learning

Key Columns
Player_Name  
Format  
Venue  
Opposition  
Runs  
Balls  
Strike_Rate  
Fours  
Sixes  
Date  

🛠️ Tools Used

Excel → Data cleaning & formatting

Python (Pandas, Matplotlib) → EDA

Power BI → Dashboard creation

📊 Dashboard Visuals
1️⃣ Average Runs per Player

Shows consistency and overall batting strength.

2️⃣ Strike Rate Analysis

Highlights players with high scoring speed and impact.

3️⃣ Venue Analysis

Explores how batting performance varies across stadiums.

🧪 Python EDA Summary

Python was used to validate trends before visualization:

Average runs per player

Strike rate distribution

Venue-wise performance

Example code snippet:

import pandas as pd

df = pd.read_excel("cricket_mixed_50.xlsx")

avg_runs = df.groupby("Player_Name")["Runs"].mean()
avg_strike = df.groupby("Player_Name")["Strike_Rate"].mean()
venue_perf = df.groupby("Venue")["Runs"].mean()

print(avg_runs)
print(avg_strike)
print(venue_perf)

🧼 Data Cleaning Steps

Removed empty rows

Ensured numeric formatting

Standardized venue and player names

Formatted dates correctly

🎯 Key Insights

Some players show high consistency (strong average runs)

High strike-rate players excel in aggressive formats like T20

Venues differ significantly in batting difficulty

Visuals clearly reveal patterns helpful for cricket analysis

🏁 Conclusion

This project demonstrates the integration of:

Excel for cleaning

Python for statistical analysis

Power BI for interactive visualization

The result is a clean, easy-to-understand dashboard focusing on batting performance analytics.

📥 Project Files

cricket_mixed_50.xlsx – dataset

.pbix – Power BI dashboard

Cricket_Batting_Dashboard_Report.docx – project report

README.md – GitHub documentation

🤝 Contributing

Contributions are welcome!
Fork the repo and submit a PR.

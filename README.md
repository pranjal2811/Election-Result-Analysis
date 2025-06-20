# Election Results 2024 Analysis Dashboard
Hello, folks! My name is Pranjal Joshi, and I am delighted to present my project. This project involved a comprehensive analysis of election results from 2024, providing valuable insights into party performance, seat distribution, and victory margins across various constituencies and states.

# Project Overview
The core of this project was to perform an in-depth analysis of election data. The primary goal was to understand various aspects of the 2024 election outcomes, including the overall distribution of seats, the performance of leading parties, state-wise party wins, and the margins of victory. The dashboard provides a dynamic and intuitive interface to explore these critical election statistics.

# Objectives
This project was developed with several key objectives to provide a comprehensive analysis of the election data:

Understand Overall Dynamics: To identify the overall dynamics of the election by calculating key performance indicators, such as the average margin of victory, the largest recorded margin, total seats, and the count of party wins by state, to understand the scale and competitiveness of the results.

Pinpoint Geographic Patterns: To pinpoint geographical patterns of party dominance by visualizing the leading party's performance across states and constituencies, revealing regional strongholds and areas of influence.

Uncover State-Level Power Distribution: To understand the distribution of political power at the state level by breaking down total seats per state and illustrating how party wins are distributed, highlighting state-specific electoral landscapes.

Identify Most Contested Races: To uncover the most contested races by identifying constituencies with the minimum winning margins, thereby highlighting areas of significant electoral competition, and to analyze overall winning party distribution to understand general trends.

Recognize Major Political Forces: To recognize the major political forces by summarizing and visualizing the performance of the top 5 leading parties, indicating their overall strength and impact on the election outcome.

Enable Targeted Investigations: To empower users with the ability to conduct targeted investigations by enabling interactive filtering of data by state and leading party, allowing for deeper, segment-specific analysis of the election results.

# Implementation Steps
I utilized Power BI Desktop for data loading, DAX calculations, and dashboard visualization.

Data Loading and Preparation:

The election_results_2024 dataset was loaded into Power BI.

The table contains columns providing information about constituencies, states, political parties, victory margins, and election status.

DAX Measure Creation:
The following crucial DAX measures were created to compute key election statistics for dynamic analysis:

Avg Margin = AVERAGE(election_results_2024[Margin])

Purpose: Calculates the average victory margin across all constituencies.

Largest Margin = MAX(election_results_2024[Margin])

Purpose: Identifies the single largest victory margin recorded in any constituency.

Party Wins by State = CALCULATE(COUNTROWS('election_results_2024'), 'election_results_2024'[Status] = "Result Declared")

Purpose: Counts the total number of constituencies where a result has been declared, representing the total party wins across all states. This measure specifically filters for only declared results.

Total Seats = COUNT(election_results_2024[Constituency])

Purpose: Calculates the total number of constituencies analyzed in the dataset, effectively representing the total number of seats.

Dashboard Visualizations:

KPI Cards: Display Average Margin (162.05K), Largest Margin (1M), Total Seats (543), and Party Wins by State (542) to offer immediate high-level insights.

Geographic Maps: An interactive map visualizes Leading party by Status and Leading party by Constituency, allowing for a clear understanding of party dominance across different regions of India.

Bar Charts:

Total Seats in Every State: Illustrates the distribution of constituencies across various states (e.g., Uttar Pradesh: 80, Maharashtra: 48).

Party Wins by State: A stacked bar chart detailing the breakdown of seats secured by different parties within each state.

Party Win with Minimum Margin by Constituency: Highlights constituencies with the closest election results (e.g., Visakhapatnam, Warangal), indicating highly competitive races.

Top 5 leading party: Presents a concise summary of the total seats won by the top 5 parties (e.g., Bharatiya Janata: 240, Indian National: 99).

Pie Chart: Winning Party by Area shows the percentage distribution of wins among different leading parties (e.g., Bharatiya Jana... 44.2%).

Interactive Filters: Slicers for Leading Party and State were implemented to provide dynamic filtering and drill-down capabilities for users.

# Results and Conclusion
The Election Results 2024 Analysis Dashboard provides a comprehensive and interactive view of the election outcomes:

Overall Summary: Key statistics like the total seats contested (543), the substantial largest margin of 1 million, and an average margin of 162.05K offer a high-level overview of the election's scale and competitiveness.

Geographic Insights: The interactive maps visually demonstrate the geographical spread of party dominance and show which parties lead in various constituencies and states.

State-wise Performance: The dashboard clearly breaks down the seat distribution per state and illustrates the specific parties that secured wins in each region, highlighting strongholds and contested areas.

Party Dominance: The "Top 5 leading party" chart quickly identifies the major players and their respective seat counts, confirming the overall power structure (e.g., Bharatiya Janata leading with 240 seats).

Close Contests: The "Party Win with Minimum Margin by Constituency" chart is crucial for pinpointing constituencies where elections were highly competitive, offering valuable insights into voter sentiment and strategic importance.

This project demonstrates proficiency in data analysis, DAX formula creation, and dashboard design using Power BI to transform raw election data into meaningful and easily digestible insights.

# Tools and Technologies Used
Power BI Desktop: Core tool for dashboard development and visualization.

DAX (Data Analysis Expressions): Utilized extensively for creating calculated measures (Avg Margin, Largest Margin, Party Wins by State, Total Seats).

# Contact Information
Name: Pranjal Joshi

GitHub: https://github.com/pranjal2811

LinkedIn: https://www.linkedin.com/in/pranjaljoshi2811

Email: pranjaljoshi2811@gmail.com

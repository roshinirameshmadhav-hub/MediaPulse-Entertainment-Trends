MediaPulse – Entertainment Content Trends Dashboard

This project was developed as part of my EURON Internship to analyze trends in media content consumption using Power BI. The goal was to uncover insights about viewership behavior, popular genres, and platform preferences through interactive data visualization.


---

Project Overview

The MediaPulse Dashboard provides a clear, data-driven view of how audiences engage with entertainment content across various platforms such as Netflix, Amazon Prime, and YouTube.
Using data from three related tables — Content, User, and Viewership — the dashboard highlights:
Most watched genres
Platform-wise audience distribution
Viewership trends over time
Gender-based and demographic insights


Data Model

Tables Used:
Table	Description
Content	Stores metadata such as Title, Genre, ReleaseDate, and Platform.
User	Contains demographic details like Age, Gender, and Location.
Viewership	Tracks who watched what and when (ViewDate).


Relationships:

Viewership[ContentID] → Content[ContentID]
Viewership[UserID] → User[UserID]


DAX Measures

Measure	Formula	Purpose
Total Views	COUNTROWS(Viewership)	Total number of viewing records
Unique Users	DISTINCTCOUNT(Viewership[UserID])	Count of distinct viewers
Content Count	DISTINCTCOUNT(Viewership[ContentID])	Total unique content titles watched



Dashboard Features

KPI Cards – Total Views, Unique Users, and Content Count
Bar Chart – Most Watched Genres
Pie Chart – Platform-wise Viewership Distribution
Line Chart – Viewership Trend Over Time
Column Chart – Demographic Breakdown by Gender

Key Insights
Series and movies dominate viewership, with strong engagement on Netflix and Amazon Prime.
Male viewers aged 18–25 represent the highest activity group.
Viewership peaks mid-month, suggesting consistent streaming habits.
The dashboard provides actionable insights for content strategy and audience targeting.


Tools & Technologies
Microsoft Power BI – Data modeling, DAX, and visualization
Microsoft Excel – Data source and preparation
GitHub – Version control and project hosting


📂 Project Files

File Name	Description
MediaPulse_Report.pbix	Power BI Dashboard file
MediaPulse_Data.xlsx	Dataset used for analysis


How to View the Dashboard
1. Download the .pbix file from this repository.
2. Open it using Power BI Desktop (free from Microsoft).
3. Explore visuals interactively — apply filters by genre, platform, or location.



*Author

 Roshini R Rao
 EURON Internship Participant
 https://www.linkedin.com/in/roshinirameshrao?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app
 Aspiring Product Manager | Data & Analytics Enthusiast



⭐ This project demonstrates my ability to transform raw data into interactive business insights using Power BI and DAX.

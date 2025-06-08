# **Social Buzz - Engagement Analysis - Bi-weekly Update**
_**Author**: Thu Pham | **Date**: 06/2025_

## *Table of Contents*
1. [Project Background](#1-project-background)  
2. [Data Structure & Initial Checks](#2-data-structure--initial-checks)  
3. [Executive Summary](#3-executive-summary)  
4. [Insights Deep Dive](#4-insights-deep-dive)  
5. [Recommendations]

## _**1. Project Background**_

<p align="center">
 <img src="images/SocialBuzz_logo_resize.png" alt="Centered Image">
</p>

This project focuses on a comprehensive data analysis of **Social Buzz**, a dynamic social media platform that has achieved remarkable growth, boasting **over 500 million active users (Monthly Active Users - MAU)** within just five years. A key differentiator for Social Buzz is its emphasis on **user anonymity**, . The platform supports a rich content ecosystem with **16 distinct content categories** and **four content formats** (GIF, audio, video, photo).

This portfolio project simulates the role of a Junior Data Analyst within a data team, responsible for monitoring and driving platform engagement. Specifically, the project involves conducting **bi-weekly engagement review meetings** to present actionable insights to product teams, content teams and marketing divisions, all of whom are invested in or responsible for enhancing platform engagement.

The analysis delves into crucial social media performance metrics and KPIs, including:

* **User Activity & Growth:** Monitor **Monthly Active Users (MAU)** and **Total Reactions** to assess platform engagement and long-term growth. 
* **Content Performance & Reach:** This objective evaluates how effectively content surfaces to and engages users, measured by the **Content Activation Rate** and the proportion of **unengaged content** over time, along with the **average daily content interactions per user**.
* **Content Quality & Sentiment:** Here, we aim to identify and categorize "power categories" versus underperforming ones by analyzing overall **positive sentiment percentages** and delving into specific **reaction types** to understand nuanced user emotional responses to content.
* **User Behavior Patterns:** This segment focuses on optimizing content delivery by pinpointing **optimal engagement windows** (e.g., by day of week and hour) and identifying activity peaks, informing tailored content scheduling strategies.

An interactive Excel Dashboard used to report can be found here [link](Social_Buzz_dashboard.xlsx)

The bi-weekly report file hypothetically used for presentation in bi-weekly meeting can be found here [link]

The presentation in video format can be found here [link].

## _**2. Data Structure & Initial Checks**_
The database structure for the meeting seen below consists of three tables:
- **`Contents`**: This dataset contains **1,000 distinct entries**, with each row representing a unique piece of content available over the past twelve months. Key attributes include a unique content ID, its associated creator (`User_id`), the content's format (e.g., video, photo), and its thematic category..
- **`Reactions`**: Comprising **approximately 25,000 rows**, this table records each user interaction with content. Every entry specifies the user (`User_id`), the `Content_id` they reacted to, the exact date and time of the reaction, and the specific type of reaction applied.
- **`ReactionsTypes`**:  This lookup table provides definitions for each reaction type available on the platform. For every reaction, it details its overall `Sentiment` (e.g., positive, neutral, negative) and assigns a `Score` that quantifies its emotional intensity. 

<p align="center">
 <img src="images/Social_Buzz_ERD.png" alt="Centered Image">
</p>

## _**3. Executive Summary**_

Social Buzz has maintained a stable base of **480-490 reacting users per month** over the past year. However, **June 2021** signals a critical challenge, with a **2% drop in active users** and a **9% decrease in total reactions**, indicating a pressing need for sustained growth initiatives.

Our analysis reveals significant gaps in content effectiveness, as only **76% of content successfully reaches audiences** in the past month, and a concerning **4% remains entirely unengaged** over a 12-month period. This is compounded by a shallow average of just **1.04 reactions per user daily**, indicating potential for deeper platform engagement.

Despite these challenges, "power categories" (e.g., 'animals', 'technology', 'science') consistently drive high **positive sentiment**, accounting for **over 57%** of total reactions, contrasting with persistent underperformers. User behavior patterns identify **peak activity on Tuesdays** and a notable 3 AM - 6 AM activity surge, highlighting clear opportunities to optimize content delivery strategies for our diverse, global user base.

## _**4. Insights Deep dive:**_
### *4.1. Main Insight 1: User interaction with the platform contents raise some problems*
- For the past 12 months (June 2020 - June 2021),480-490 active on the platform per month, only 60 audiences daily and each of them only interact with 01 post a day.
- 96% contents pieces reach the audiences 
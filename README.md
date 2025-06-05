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



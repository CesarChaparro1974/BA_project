# Internship in the analytical department at Yandex.Afisha.

## Task
* To help optimize marketing expenses. 

### We have:

1. Server logs with data on Yandex.Afisha visits from June 2017 through May 2018
2. Dump file with all orders for the period
3. Marketing expenses statistics

### I study:

1. How people use the product
2. When they start to buy
3. How much money each customer brings
4. When they pay off

### Steps

1. Download the data and prepare it for analysis
   - Stored the data on visits, orders, and expenses in variables. Optimized the data for analysis. Made sure each column contains the correct data type. 
2. Make reports and calculate metrics:<br>
   2.1. Product:<br>
      - How many people use it every day, week, and month?
      - How many sessions are there per day? (One user might have more than one session.)
      - What is the length of each session?
      - What's the user retention rate?<br>
   2.2. Sales:<br>
      - When do people start buying? (In KPI analysis, we're usually interested in knowing the time that elapses between registration and conversion — when the user becomes a customer. For example, if registration and the first purchase occur on the same day, the user might fall into category Conversion 0d. If the first purchase happens the next day, it will be Conversion 1d. You can use any approach that lets you compare the conversions of different cohorts, so that you can determine which cohort, or marketing channel, is most effective.)
      - How many orders do they make during a given period of time?
      - What is the average purchase size?
      - How much money do they bring? (LTV)<br>
   2.3. Marketing:<br>
      - How much money was spent? Overall, per source and over time.
      - How much did customer acquisition from each of the sources cost?
      - How worthwhile where the investments? (ROI)
* There are plot graphs to display how these metrics differ for various devices and ad sources and how they change in time.

3. There is a conclusion: advised marketing experts how much money to invest and where:
  * What sources/platforms do I recommend? Backed up the choice by: what metrics did I focus on? Why? What conclusions did I draw after finding the metric values?
  * Format: Completed the task in Jupyter Notebook.

### Description of the data
1. The visits table (server logs with data on website visits):
   - Uid — user's unique identifier
   - Device — user's device
   - Start Ts — session start date and time
   - End Ts — session end date and time
   - Source Id — identifier of the ad source the user came from
* All dates in this table are in YYYY-MM-DD format.
2. The orders table (data on orders):
  - Uid — unique identifier of the user making an order
  - Buy Ts — order date and time
  - Revenue — Yandex.Afisha's revenue from the order
3. The costs table (data on marketing expenses):
  - source_id — ad source identifier
  - dt — date
  - costs — expenses on this ad source on this day


### Installing 
* Clone the Repo and run npm install and npm run to run on localhost

[Click here to see live Version --> ](https://newmovies.netlify.app)

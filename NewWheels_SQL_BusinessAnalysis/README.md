# New Wheels — SQL Business Analytics

## Problem Statement
New-Wheels, a vehicle resale company, has seen steadily declining sales and a drop in new customers. As a data analyst, the task is to answer a set of leadership-level business questions using SQL and compile the findings into a quarterly business report for the CEO.

## Approach
Wrote SQL queries against a multi-table relational database (customers, orders, products) to answer 10 business questions covering customer distribution, vehicle maker preferences, feedback trends, revenue, and shipping performance. Used JOINs across tables, window functions (RANK, LAG) for ranking and quarter-over-quarter comparisons, and CASE logic for feedback scoring. Consolidated findings into a business metrics overview and a prioritized set of recommendations.

## Key Findings
- Orders and net revenue declined ~36–40% from Q1 to Q4
- Average shipping time tripled (57 → 174 days), strongly correlated with declining customer satisfaction
- "Bad"/"Very Bad" feedback rose from ~22% to ~59% of responses over the year

## Skills
Complex SQL querying (multi-table joins, subqueries), window functions (RANK, LAG), date arithmetic, KPI derivation, business report writing

## Tech Stack
SQL

## Dataset
New-Wheels transactional database dump, provided as part of PGP-AIML coursework.

# Office-Supply-Analysis

## Overview

This repository contains a SQL case study built around the Office Supply domain—focusing on customer purchasing behaviour, product usage, subscription patterns, and support operations. The exercises strengthen essential SQL concepts such as aggregation, joins, filtering, date logic, window functions, and conditional calculations.
All questions mirror realistic analytics tasks that a business analyst or data analyst would tackle in a retail or product-based environment.

## Key Features

* Domain-focused SQL tasks using real-world objects: customers, users, purchases, sessions, subscriptions, and support tickets.
* Business questions rewritten around office-supply tools (Stapler, Notepad, Highlighter, Binder, Ballpoint Pen).
* Clear mapping from stakeholder-style questions to SQL solutions involving grouping, subqueries, retention logic, and time-based comparisons.

Includes examples of:

* Conditional aggregation (**CASE WHEN**)
* Date **filtering** and rolling windows (last 12 months)
* Median calculation using **window** functions
* Upgrade path detection using **self-joins**
* Quarter-over-quarter ticket analysis
* MySQL-compatible queries with easy portability to PostgreSQL.

## Dataset

This project uses a compact analytical schema representing a small office-supply business universe.

* **customers** — Customer accounts, including type (enterprise/individual) and region.
* **users** — End users linked to customer accounts, with signup and last login info.
* **purchases** — Line-level product purchases across tools such as Stapler, Notepad, Highlighter, Binder, and Bulk Binder Pack.
* **sessions** — User engagement sessions tied to specific products.
* **subscriptions** — Membership plans (Single Item and All Tools), including upgrades and cancellations.
* **support_tickets** — Product-related support issues with timestamps and resolution times.

This dataset is intentionally kept small and interpretable so the focus remains on SQL reasoning rather than data size.

## How to Use

1. **Clone** this repository.
2. **Load the schema and sample data** from the /sql folder into your MySQL or PostgreSQL environment.
3. **Run the 10 practice questions** in the queries/ folder, each representing a real analytic scenario.
4. **Review the SQL solutions** to compare approaches or validate your own results.
5. **Extend the dataset** with more products, regions, or time ranges to deepen your analysis.
6. **Adapt syntax** as needed for your SQL engine (MySQL and PostgreSQL both supported with minor adjustments).

## Insights You Can Find

* **Product analytics**

  * Top-selling items (Stapler, Notepad, Highlighter, etc.) over rolling 12-month windows.
  * Cross-product purchasing behaviour (e.g., customers who buy Highlighters but not Bulk Binder Packs).
  * Enterprise customer spend patterns and identification of high-value accounts.

* **Usage & engagement**

  * Average session duration for specific products by user location.
  * Understanding user activity after signup to support onboarding analysis.

* **Subscriptions**

  * Median subscription value to evaluate pricing distribution.
  * Detection of customers upgrading from Single Item plans to All Tools bundles.

* **Support operations**

  * Quarter-over-quarter ticket trends by product.
  * Identification of products experiencing >20% increase in support load.
  * These exercises simulate true stakeholder requests and build analytical depth suitable for interviews, dashboards, and day-to-day business reporting.

## Tools & Technologies

* SQL (MySQL + PostgreSQL compatible)
* DBeaver, MySQL Workbench, pgAdmin, or any SQL IDE
* Git & GitHub for version management and portfolio building

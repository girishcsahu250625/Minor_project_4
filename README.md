# Minor_project_4

BingePlay Analytics: End-to-end SQL &amp; Python analysis querying a MySQL OTT streaming database. Analyzes active subscriptions, monthly revenue, device watch time, rating distributions, original vs. acquired show performance, user binge/streak behaviors, plan upgrades, and May-to-June churn risk signals.

Project Overview

This repository contains end-to-end data pipelines and SQL queries executed via Python (`pandas` & `sqlalchemy`) against a MySQL database (`bingeplay`). The analysis covers key business metrics spanning the first half of 2024 (January to June 2024), including:

* Revenue & Growth:** Tracking active subscriptions, total monthly recurring revenue (MRR), and monthly user signups.
* Content & Platform Performance:** Evaluating device-level watch time, completion rates, rating distributions, and comparing *BingePlay Originals* vs. *Acquired Content*.
* User Engagement Patterns:** Identifying power users through binge-watching behaviors, weekly streaming streaks, and comeback activity post-unfinished sessions.
* Retention & Churn Risk:** Pinpointing over-paying users, average days to plan upgrades, and flagging potential churn risks based on month-over-month watch time drops.

Key Insights Analyzed

* Active Subscriptions & Revenue:** Calculates active subscriber counts and evaluates total monthly revenue in INR.
* Sign-up Trends:** Tracks monthly registration patterns to identify peak acquisition months (May and June saw the highest sign-up volume).
* Device Usage:** Analyzes session volume, total watch minutes, average session duration (~30 mins), and completion rates (~60%) across Laptops, Mobiles, Tablets, and TVs.
* Content Quality & Originals:** Compares IMDb ratings and release years between acquired shows and BingePlay Originals (Originals average a higher IMDb score of ~7.92).
* User Engagement Streaks:** Detects users with 4+ consecutive week streaming streaks and highlights top binge-watching behavior (users completing 5+ sessions of a single show in a day).
* Churn Signal Detection:** Flags high-risk users who experienced a $\ge 50\%$ drop in watch minutes between May and June 2024.

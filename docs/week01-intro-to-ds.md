---
title: "Week 1 – Introduction to Data Science"
description: "Executive summary, case studies (Netflix/Blockbuster/Zillow), descriptive vs. predictive, and thinking statistically."
authors: ["Daniel B. Altieri"]
date: "2026-01-27"
tags: ["introduction","data science","predictive analytics","descriptive statistics"]
toc: true
---

# Week 1 – Introduction to Data Science

> **TL;DR**: Data science creates value when it aligns with decisions. Learn to define the problem, measure well, summarize variation (not just averages), and build predictions with explicit assumptions. Failures (e.g., Blockbuster) often reflect **assumption breaks** and measurement gaps—not just bad models.

**See also:** Week 2 · Reliability vs. Validity

## Executive Summary {#executive-summary}

Data science is central to modern decision-making, with organizations using analytics to drive success.

- **Netflix**: Leveraged data to transform its business model and achieve massive growth.
  - Applications: Recommendation systems, user engagement prediction, operational efficiency.
- **Blockbuster**: Failed to adapt to data analysis → Decline and bankruptcy.

**Successes and Failures in Data Science**
- **Netflix**: Embedded analytics into core operations → Success.
- **Zillow**: Predictive models for home buying failed due to unexpected changes in housing and construction costs → $420M loss.
- **Lesson**: Models are only as good as the data and assumptions behind them.

**Key Concepts: Models, Variables, and Prediction**
- **Dependent Variables**: Outcomes of interest (e.g., subscription length, home price).
- **Independent Variables**: Predictors (e.g., past viewing habits, neighborhood characteristics).
- **Models**: Establish relationships between predictors and outcomes → Enable prediction and decision-making.

**Descriptive and Predictive Analysis**
- **Descriptive Analysis**: Summarizes patterns in data (central tendency, variation).
- **Predictive Modeling**: Forecasts outcomes based on variable relationships.
- **Goal**: Generate actionable insights for decision-making.

## Lecture 1: Introduction to Data Science {#lecture-1}
- Netflix’s transformation through analytics: From DVD mail service → Streaming giant.
- Predictive analytics for engagement and membership retention.
- Engineering predictions for server load and content delivery.
- Visualization for actionable insights across teams.
- Blockbuster’s failure: Ignored predictive modeling → Bankruptcy.
- Zillow’s failure: Predictive models didn’t account for unprecedented construction cost increases → Huge losses.
- **Core Idea**: Prediction is hard—especially about the future. Models fail when assumptions break.

## Lecture 2: Course Overview {#lecture-2}

**Course Design and Focus**
- Emphasis on decision-making over technical skills.
- Students learn: Data structures and measurement; Modeling and prediction; Effective presentation of analysis.

**Data Structures and Measurement**
- Turning real-world phenomena into measurable variables.
- Continuous vs. categorical variables.
- Challenges in measuring abstract concepts (e.g., personality traits).

**Modeling and Prediction**
- Linear and classification models.
- Advances in AI and large language models → Intuitive understanding.

**Presentation of Data Analysis**
- Importance of clear communication for decision-makers.
- Choosing appropriate summary measures and visualizations.

**Assignments and Tools**
- Bi-weekly assignments + final project using Excel (or other tools).
- Focus: Applying concepts to organizational decision-making.

## Lecture 3: Key Problems in Data Science Projects {#lecture-3}

- **Defining Important Problems**: Start with why the problem matters and who it affects. Avoid methodology-driven projects or competitive mimicry.
- **Pitfalls in Data Collection and Measurement**: Sampling only on successful outcomes; lack of variation; assuming causality; misalignment between concepts and measurements.
- **Project Completion and User Focus**: Define success upfront; avoid proving pet hypotheses; link analysis results to specific decisions.
- **Trust and Engagement with Data**: Engage users early; design for decision-makers.

## Lecture 4: Thinking Statistically {#lecture-4}

- **Asking the Right Questions**: Where does the data come from? Universe vs. convenience vs. random sample.
- **Purpose of Data Analysis**: Describe, infer, predict.
- **Central Tendency and Variation**: Consider dispersion alongside averages (e.g., income distribution vs. mean).
- **Probability, Inference, and Prediction**: How wrong might the model be?

## FAQ {#faq}

**Q: Why did Zillow’s model fail if it used lots of data?**  
**A:** Large, sudden shifts in construction and market dynamics broke key assumptions; the training signal no longer matched reality. Models are only as strong as their **assumptions and data-generating process**.

**Q: Is descriptive analysis enough for decision-making?**  
**A:** Sometimes. Start with **descriptive summaries** to understand patterns and variation; move to **prediction** only when you need forecasts to choose between actions.

**Q: What’s the quickest way to build trust with stakeholders?**  
**A:** Engage early, define success criteria together, and present results in decision-ready formats (clear comparisons, uncertainty, and implications).

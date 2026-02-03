---
title: "Week 5 – Survey Data and Analysis"
description: "Study notes on survey design, sampling, weights, GSS, question types, data structure, and crosstab analysis."
authors: ["Daniel B. Altieri"]
date: "2026-01-27"
tags: ["survey","GSS","weights","crosstab","question design"]
toc: true
---

# Week 5 – Survey Data and Analysis

> **TL;DR**: Generalize with **probability samples** and **weights**; always read the **codebook**. For crosstabs: put **IV on rows**, **DV on columns**, and use **row %** to compare groups. Separate **demographic**, **behavioral**, and **attitudinal** variables. Design questions with clarity and mutually exclusive options.

**See also:** Week 2

## 1. What Is Survey Data?
Survey data is collected by asking people questions and recording their responses. It allows systematic information gathering about behaviors, attitudes, and demographics—especially when direct observation is impractical.

## 2. Sampling in Survey Research
### 2.1 Samples vs. Populations
We survey a **sample** (subset) to draw inferences about a **population**.

### 2.2 Probability Sampling
A probability sample has known selection probabilities, enabling generalization beyond respondents.

### 2.3 Survey Weights
When selection probabilities differ, **weights** adjust estimates so each respondent represents the correct number of people. Large surveys (e.g., **GSS**) rely on weights.

## 3. The General Social Survey (GSS)
- Long‑running national survey of U.S. adults, with consistent methods across decades.
- Collects education, health behaviors, social attitudes, etc.
- **Codebooks** document variable construction, skip patterns, and response options; always consult them.

## 4. Types of Survey Questions
- **Open‑Ended**: nuanced but hard to quantify.
- **Closed‑Ended / Multiple Choice**: standardized and efficient for quantitative analysis.
- Other formats: ranking, forced‑choice, sliders—use with care.

## 5. Categories of Survey Variables
- **Demographic** (often IVs): stable characteristics (e.g., education, age).
- **Behavioral**: actions within time windows (e.g., doctor visits, voting).
- **Attitudinal**: beliefs, opinions, values; distinct from behavior.

## 6. Question Design Principles
- Keep questions concise and focused.
- Avoid leading/loaded wording; use clear language.
- Provide complete, mutually exclusive options.
- Do not mix behaviors and attitudes in one question.

## 7. Structure of Survey Data Files
- Rectangular datasets: rows = respondents; columns = variables.
- Numeric codes may label categories; do **not** treat as quantities unless appropriate.

## 8. Crosstabulation (Core Analysis Tool)
**What**: Compare two categorical variables to reveal association.

**Best practice**
- Place **independent variable on rows**; **dependent on columns**.
- Use **row percentages** to compare groups.

## FAQ

**Q: When must I apply survey weights?**  
**A:** When selection probabilities differ (most complex/national surveys). Weights restore population representativeness.

**Q: Why row percentages (not column) in crosstabs?**  
**A:** With IV on rows, row % let you compare **groups of interest** directly on the DV distribution.

**Q: How do I handle “Not asked / Inapplicable” vs. missing?**  
**A:** Use **explicit codes** and exclude inapplicable cases from denominators to avoid biased percentages.

---
title: "Reliability and Validity in Research Design"
subtitle: "Structured Lecture Narrative"
author: "Extracted and structured from course lecture transcript"
date: "2026-01-27"
toc: true
toc-depth: 3
---

## Introduction

This lecture introduces two foundational concepts in research methodology: **reliability** and **validity**. While both are central to the quality of scientific measurement, they answer different questions. Reliability concerns **consistency**, whereas validity concerns **truth**—whether a measure actually captures what it claims to measure.

The session revisits familiar ideas, reframes others, and introduces new distinctions that will be important for interpreting results, evaluating studies, and designing sound measures.

---

## Reliability vs. Validity: Core Distinction

### What Is Reliability?

Reliability refers to the **degree of consistency or repeatability** in measurement. A reliable measure yields similar results when:

- Repeated over time  
- Used by different observers  
- Administered using equivalent forms  

In short, reliability asks: *Do we get similar answers each time we measure the same thing?*

### What Is Validity?

Validity refers to the **degree to which a measure reflects the truth**. A valid measure accurately captures the construct it is intended to assess.

Validity asks: *Are we measuring the correct thing?*

### Reliability and Validity Illustrated

A common visualization is a **target diagram**:

- Each dot represents a measurement.
- The bullseye represents the true value.

From this illustration, we can observe four possible situations:

- **Unreliable and invalid:** Measurements are scattered and far from the center.
- **Reliable but invalid:** Measurements cluster tightly but miss the bullseye.
- **Valid but unreliable:** Measurements are spread out but average near the center.
- **Reliable and valid:** Measurements are tightly clustered around the center.

---

## Why Reliability and Validity Matter

The importance of reliability and validity is straightforward:

- We want tools that are **consistent**.
- We want tools that measure **what they are supposed to measure**.

Without reliability, results are unstable. Without validity, results are meaningless—even if they are consistent.

---

## Types of Reliability

When researchers assess reliability, they typically focus on four major types.

---

### Inter‑Rater (Inter‑Observer) Reliability

Inter‑rater reliability concerns **agreement between multiple raters or observers**.

This type of reliability is most relevant when researchers record or code observations, whether in naturalistic settings or laboratory environments.

#### How It Is Calculated

- **Categorical data:**  
  Percentage agreement between raters.
- **Continuous data:**  
  Correlation between raters' scores.

#### Example: Inter‑Rater Reliability

Two raters evaluate five items.

- **Categorical example:**  
  Reliability is calculated as the proportion of agreements (e.g., 4 out of 5 = 0.80).

- **Continuous example:**  
  Reliability is assessed using Pearson's correlation (e.g., *r* = 0.83).

> Note: Inter‑rater reliability is vulnerable to threats such as rater drift and inadequate training, which will be addressed in later lessons.

---

### Test–Retest Reliability

Test–retest reliability evaluates **consistency across time**.

The same measure is administered to the same participants at two different time points. High reliability is indicated by stable scores over time.

#### Calculation

- **Categorical variables:** Percentage agreement  
- **Continuous variables:** Correlation between time points

#### Example: Test–Retest Reliability

Participants are measured at Time 1 and Time 2.

- A strong correlation between total scores across time indicates high reliability.
- Low agreement suggests instability in the measurement.

---

### Parallel Forms Reliability

Parallel forms reliability involves creating **equivalent versions of a test**.

#### Procedure

1. Begin with a large pool of items.
2. Divide items into separate forms:
   - Randomly, or
   - Using item characteristics such as difficulty and sensitivity.
3. Treat forms as interchangeable.

A person scoring 10 on Form A should score approximately 10 on Form B.

#### Example: Parallel Forms

Scores from Form 1 and Form 2 are compared across participants.

- High correspondence is expected.
- Low correspondence indicates the forms are not truly equivalent.

Parallel forms reliability is most common in **test construction** and is relatively rare in applied research.

---

### Internal Consistency Reliability

Internal consistency examines **how well items within a single measure relate to one another**.

This is the most common form of reliability reported in psychological research.

#### Average Inter‑Item Correlation

- Compute correlations among all items.
- Average the off‑diagonal correlations.

#### Item–Total (Part–Whole) Correlations

- Correlate each item with the total score.
- Average the resulting correlations.

#### Cronbach's Alpha

Cronbach's alpha represents the **average of all possible split‑half reliabilities**.

##### Conceptual Explanation

1. Split items into two halves.
2. Correlate the two total scores.
3. Repeat for all possible splits.
4. Average the results.

Modern statistical software (e.g., R, SPSS, Excel) computes Cronbach's alpha automatically.

---

## From Reliability to Validity

Reliability is ultimately a **threshold question**: Is consistency "close enough"?

Validity is more complex. It asks a harder question: *Are we measuring what we think we're measuring?* This makes validity more abstract and, in some cases, unavoidably subjective.

---

## Types of Validity

Validity can be organized into two broad families:

- **Inference‑Based Validity**
- **Construct‑Based Validity**

---

## Inference‑Based Validity

### Internal Validity

Internal validity asks whether the **study design** justifies the conclusions drawn.

Key questions include:

- Were extraneous variables controlled?
- Were alternative explanations ruled out?
- Did the study proceed as planned?

### External Validity

External validity concerns **generalizability**.

It asks whether findings extend:

- Beyond the specific sample
- Beyond the experimental conditions
- To real‑world contexts

---

## Construct‑Based Validity

Construct validity addresses whether a measure meaningfully represents the theoretical construct of interest.

It includes two main categories.

---

### Translational Validity

Translational validities involve subjective judgment.

#### Face Validity

Does the measure *look like* it assesses the intended construct?

#### Content Validity

Does the measure adequately sample the full domain of the construct?

Example:  
A test of intelligence should capture multiple facets—not just a narrow slice.

---

### Criterion Validity

Criterion validity assesses how a measure relates to other variables.

#### Predictive Validity

Does the measure predict outcomes it should theoretically predict?

#### Concurrent Validity

Does the measure correlate with other established measures administered at the same time?

#### Convergent Validity

Does the measure correlate with related constructs it should be associated with?

Example:  
An intelligence measure correlating with academic performance.

#### Discriminant Validity

Does the measure **not** correlate with constructs it should be unrelated to?

Example:  
An intelligence measure correlating with shoe size would indicate a problem.

---

## Interpreting Criterion Validity

Criterion validity relies on **correlations**, but interpretation is nuanced.

There are no absolute thresholds for:

- How large a correlation must be for convergent validity.
- How small a correlation must be for discriminant validity.

Judgment is required to determine whether observed correlations are meaningful or negligible. As a result, validity—unlike reliability—cannot be fully reduced to a single number.

---

## Conclusion

This lecture establishes crucial terminology and conceptual distinctions needed for evaluating measurement quality. While reliability focuses on consistency and offers relatively concrete metrics, validity addresses the deeper question of meaning and truth in measurement.

These foundations will support later discussions of **construct validation** and **critical multiplism**, where multiple traits and methods are used to more rigorously test whether our measures behave as theory predicts.

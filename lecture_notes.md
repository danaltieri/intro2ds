# Lecture Transcript and Notes  
## Week 1  

---

## Executive Summary  

### **Introduction to Data Science**  
Data science is central to modern decision-making, with organizations using analytics to drive success.  
- **Netflix**: Leveraged data to transform its business model and achieve massive growth.  
    - Applications: Recommendation systems, user engagement prediction, operational efficiency.  
- **Blockbuster**: Failed to adapt to data analysis → Decline and bankruptcy.  

### **Successes and Failures in Data Science**  
- **Netflix**: Embedded analytics into core operations → Success.  
- **Zillow**: Predictive models for home buying failed due to unexpected changes in housing and construction costs → $420M loss.  
    - **Lesson**: Models are only as good as the data and assumptions behind them.  

### **Key Concepts: Models, Variables, and Prediction**  
- **Dependent Variables**: Outcomes of interest (e.g., subscription length, home price).  
- **Independent Variables**: Predictors (e.g., past viewing habits, neighborhood characteristics).  
- **Models**: Establish relationships between predictors and outcomes → Enable prediction and decision-making.  

### **Descriptive and Predictive Analysis**  
- **Descriptive Analysis**: Summarizes patterns in data (central tendency, variation).  
- **Predictive Modeling**: Forecasts outcomes based on variable relationships.  
- Goal: Generate actionable insights for decision-making.  

---

## Lecture 1: Introduction to Data Science  
**Source**: [YouTube Video](https://www.youtube.com/watch?v=Nzf8dz7mHv4&t=25s)  

### **Key Points**  
- Netflix’s transformation through analytics:  
    - From DVD mail service → Streaming giant.  
    - Predictive analytics for engagement and membership retention.  
    - Engineering predictions for server load and content delivery.  
    - Visualization for actionable insights across teams.  
- Blockbuster’s failure: Ignored predictive modeling → Bankruptcy.  
- Zillow’s failure: Predictive models didn’t account for unprecedented construction cost increases → Huge losses.  
- **Core Idea**: Prediction is hard—especially about the future. Models fail when assumptions break.  

---

## Lecture 2: Course Overview  
**Source**: [YouTube Video](https://youtu.be/yAN9_aTLavc)  

### **Course Design and Focus**  
- Emphasis on **decision-making** over technical skills.  
- Students learn:  
    - Data structures and measurement.  
    - Modeling and prediction.  
    - Effective presentation of analysis.  

### **Data Structures and Measurement**  
- Turning real-world phenomena into measurable variables.  
- Continuous vs. categorical variables.  
- Challenges in measuring abstract concepts (e.g., personality traits).  

### **Modeling and Prediction**  
- Linear and classification models.  
- Advances in AI and large language models → Intuitive understanding.  

### **Presentation of Data Analysis**  
- Importance of clear communication for decision-makers.  
- Choosing appropriate summary measures and visualizations.  

### **Assignments and Tools**  
- Bi-weekly assignments + final project using Excel (or other tools).  
- Focus: Applying concepts to organizational decision-making.  

---

## Lecture 3: Key Problems in Data Science Projects  
**Source**: [YouTube Video](https://youtu.be/KDSwKaxEgyc)  

### **Defining Important Problems**  
- Start with **why the problem matters** and **who it affects**.  
- Avoid methodology-driven projects or competitive mimicry.  

### **Pitfalls in Data Collection and Measurement**  
- Sampling only on successful outcomes.  
- Lack of variation in variables.  
- Assuming causality without evidence.  
- Misalignment between concepts and measurements.  

### **Project Completion and User Focus**  
- Define success upfront.  
- Avoid proving pet hypotheses.  
- Link analysis results to specific decisions.  

### **Trust and Engagement with Data**  
- Executives and leadership often doubt data integrity and usefulness.  
- Early engagement and user-focused design build trust.  

---

## Lecture 4: Thinking Statistically  
**Source**: [YouTube Video](https://youtu.be/2vFWkJcjPOo)  

### **Asking the Right Questions**  
- Where does the data come from?  
    - Universe of data vs. convenience sample vs. random sample.  

### **Purpose of Data Analysis**  
- Describe what’s present.  
- Infer characteristics of a larger population.  
- Predict future outcomes.  

### **Central Tendency and Variation**  
- Always consider **variation** alongside averages.  
- Example: Income distribution vs. mean income.  

### **Probability, Inference, and Prediction**  
- **Probability**: Abstract models of the world.  
- **Inference**: Use sample data to draw conclusions about populations.  
- **Prediction**: Forecast future outcomes based on observed relationships.  
    - Always ask: *How wrong is the model likely to be?*  
## Week 2
## Executive Summary: Variable Classification, Summary Statistics, and Inferential Decision Rules

### 1. Variable Classification
A variable must exhibit variation across cases. Classify variables first by type—Qualitative (Categorical) vs. Quantitative (Numeric)—and then by scale of measurement: Nominal, Ordinal, Interval, or Ratio. This classification guides appropriate statistical procedures.

![Variable classification hierarchy and scales of measurement.](images/figure1.png)

**Examples:**
- Number of votes → Quantitative, Ratio (meaningful zero).
- Highest degree achieved → Qualitative, Ordinal.
- Men’s pants sizes → Quantitative, Ratio.
- Women’s jeans sizes → Qualitative, Ordinal (labels; inconsistent numeric steps).
- Language proficiency → Depends on measurement instrument (numeric test score vs. categorical level).

### 2. Summary Statistics

**Key measures and formulas (plain text):**
- Mean (arithmetic average): `x̄ = (1/n) * Σ(xᵢ)`
- Median: middle value when ordered; for even `n`, median = `(x_(n/2) + x_(n/2+1))/2`
- Sample variance: `s^2 = Σ(xᵢ - x̄)^2 / (n - 1)`
- Sample standard deviation: `s = √(s^2)`
- Population variance: `σ^2 = Σ(xᵢ - μ)^2 / n`
- Skewness (Fisher–Pearson): `g1 = m3 / s^3`, where `m3 = mean((x - x̄)^3)`
- Excess kurtosis (Fisher): `g2 = m4 / s^4 - 3`, where `m4 = mean((x - x̄)^4)`

![Histogram visualizing distribution, central mass, and skew.](images/figure2.png)

![Boxplot highlighting median, quartiles, and potential outliers.](images/figure3.png)

#### Worked Example: Computing Summary Statistics and a 95% CI for the Mean
Given a sample (`n = 200`), we compute:
- Sample mean (`x̄`) = **52.144**
- Sample median = **51.411**
- Sample variance (`s^2`) = **145.968**
- Sample std. dev. (`s`) = **12.082**
- Skewness (`g1`) ≈ **0.827**
- Excess kurtosis (`g2`) ≈ **1.340**

**95% Confidence Interval for the mean (normal approximation):** `CI = x̄ ± z_(0.975) * SE(x̄)`, where `SE(x̄) = s/√n`, `z_(0.975) = 1.96`  
**Result:** `[50.470, 53.819]`

### 3. Inferential Statistics & Decision Rules
Summary vs. inference: Summary statistics describe a sample; inferential methods test hypotheses and estimate parameters to generalize to populations.

**Hypothesis Testing Framework:**
- `H0` (null): baseline claim (e.g., no difference).
- `H1` (alternative): competing claim.
- **Test statistic**: function of data; compare to reference distribution.
- **Decision rule**: Reject `H0` if *p*-value ≤ `α` or if test statistic exceeds critical value.

**Common procedures by scenario:**
- Two-group mean comparison (DV quantitative, IV categorical with 2 levels): **independent-samples t-test**.
- Multi-group mean comparison (DV quantitative, IV categorical with ≥3 levels): **ANOVA**.
- Association between two quantitative variables: **Pearson correlation**; **simple/multiple linear regression**.
- DV binary: **Logistic regression**; association between categorical variables: **Chi-square test**.

![Decision flow for selecting an analysis based on DV/IV types.](images/figure4.png)

### Worked Example: Choosing a Test
Scenario: Compare average training scores (numeric) between two departments (categorical: A vs. B).  
Classification → **DV quantitative**, **IV categorical (2 levels)** ⇒ **independent-samples t-test**.  
Decision rule (`α = 0.05`): reject `H0` if `t > t_crit` or `p-value ≤ 0.05`.

#### 4. Practical Guidance
Focus on conceptual correctness: choose procedures that match variable type and scale. Deviations from standard heuristics can be justified if intentional and principled.

**Checklist:** confirm variables, identify scales, specify DV/IV, choose test via decision rules, inspect assumptions (normality, homoscedasticity, independence).










































































































































































































































































































































## Week4
---
title: "Construct Validation Through the Multitrait–Multimethod Matrix(MTMM) Lens"
subtitle: "A Narrative Based on Campbell & Fiske (1959)"
author: "Prepared for teaching and reference use"
date: "2026-01-27"
toc: true
toc-depth: 3
geometry: margin=1in
fontsize: 11pt
---

### Introduction

This lesson explores a seminal approach to construct validation introduced by **Campbell & Fiske (1959)**: the **Multitrait–Multimethod (MTMM) Matrix**. Their work formalized the ideas of **convergent** and **discriminant validity**, motivated the philosophical stance of **critical multiplism**, and highlighted how much “lives inside” any single correlation—namely, contributions from **trait**, **method**, and **error**.

This narrative will:

- Revisit **critical multiplism** and why variance in methods and traits is essential  
- Explain the **MTMM matrix** and the **ideal pattern** of correlations it should reveal  
- Add **LaTeX equations** to unpack why those ideal patterns follow from variance/covariance decomposition  
- Walk through **examples**, including a synthetic illustration and a real empirical application  
- Offer **practical guidance** for using MTMM when validating a measure or inventory  

---

## Critical Multiplism: Why Vary What You Can

**Critical multiplism** argues that researchers should introduce **variance wherever possible**. If it is feasible to vary:

- stimuli  
- methods  
- measures  
- variables  
- hypotheses  

then doing so strengthens scientific inference.

The goal is twofold:

1. **Increase generalizability** by demonstrating that findings hold across different operationalizations.  
2. **Identify boundaries** by learning where results fail to generalize and why.

Rather than relying on a single method or measure, critical multiplism embraces diversity in research design to better understand constructs.

---

## The Multitrait–Multimethod (MTMM) Matrix

Campbell and Fiske proposed the MTMM matrix as a systematic way to evaluate **construct validity**. The matrix is built by:

- Measuring **multiple traits**
- Using **multiple methods**
- Computing all intercorrelations among trait–method combinations

### Core Assumptions

- **Traits should be conceptually independent** (i.e., not highly correlated).
- **Methods should be independent** (i.e., not share systematic variance beyond method effects).

This design allows researchers to:

- Separate **trait variance** from **method variance**
- Evaluate **reliability**, **convergent validity**, and **discriminant validity**
- Identify **method effects** such as response bias or testing format artifacts

---

## Interpreting an MTMM Matrix: Ideal Criteria

### Key Correlation Types

- **Reliability diagonal (mono-trait, mono-method):**  
  Correlations of the same trait measured by the same method (e.g., test–retest, parallel forms), or reported reliability estimates for that trait–method measure.

- **Convergent validity diagonal (mono-trait, hetero-method):**  
  Correlations of the same trait measured using different methods.

- **Heterotrait–heteromethod (HTHM):**  
  Correlations of different traits measured with different methods.

- **Heterotrait–monomethod (HTMM):**  
  Correlations of different traits measured using the same method.

---

### Ideal MTMM Patterns

An ideal MTMM matrix meets the following criteria:

1. **High reliability diagonals**  
   - Reliability correlations should be close to **1.0**, indicating consistent measurement.

2. **Positive convergent validity diagonals**  
   - Same traits measured by different methods should correlate **above zero**.

3. **Ordered magnitudes**  
   - **Reliability > Convergent validity > HTHM correlations**.

4. **Trait dominance over method**  
   - A **trait measured by different methods** should correlate more strongly than **different traits measured by the same method**.

5. **Consistency across hetero-method blocks**  
   - Patterns among hetero-method correlations should be stable; large deviations warrant further investigation.

> **Note:** A verbal slip in the transcript stated reliability diagonals should be “close to zero.” Conceptually, they should be **close to one**.

---

## Why These Patterns Matter: Variance/Correlation Decomposition (with LaTeX)

We can formalize why these patterns are expected by decomposing observed scores into **trait**, **method**, and **error** components.

### Score and Variance Decomposition

Let \( X_{tm} \) denote an observed score for **trait** \( t \) measured by **method** \( m \). Decompose it as:

\[
X_{tm} \;=\; T_t \;+\; M_m \;+\; E_{tm}
\]

The variance of \( X_{tm} \) is:

\[
\mathrm{Var}(X_{tm}) \;=\; \sigma_{T_t}^2 \;+\; \sigma_{M_m}^2 \;+\; \sigma_{E_{tm}}^2 \;+\; 2\,\mathrm{Cov}(T_t, M_m) \;+\; 2\,\mathrm{Cov}(T_t, E_{tm}) \;+\; 2\,\mathrm{Cov}(M_m, E_{tm})
\]

Under the simplifying assumption that **trait**, **method**, and **error** are pairwise uncorrelated:

\[
\mathrm{Var}(X_{tm}) \;=\; \sigma_{T_t}^2 \;+\; \sigma_{M_m}^2 \;+\; \sigma_{E_{tm}}^2
\]

Classical reliability (relative to a latent true score) can be expressed as:

\[
\text{Reliability}(X_{tm}) \;=\; \rho_{X_{tm}X_{tm}} \;=\; \frac{\sigma_{T_t}^2}{\sigma_{T_t}^2 + \sigma_{M_m}^2 + \sigma_{E_{tm}}^2}
\]

In a **test–retest or parallel-forms** setting with the **same method** \( m \), both trait and method components are shared across administrations, so the reliability-type correlation is expected to be highest.

### Convergent Validity (Same Trait, Different Methods)

For two methods \( m_1 \) and \( m_2 \) measuring the same trait \( t \):

\[
\begin{aligned}
X_{t m_1} &= T_t + M_{m_1} + E_{t m_1} \\
X_{t m_2} &= T_t + M_{m_2} + E_{t m_2}
\end{aligned}
\]

Their covariance is:

\[
\mathrm{Cov}(X_{t m_1}, X_{t m_2}) \;=\; \sigma_{T_t}^2 \;+\; \mathrm{Cov}(M_{m_1}, M_{m_2}) \;+\; \mathrm{Cov}(E_{t m_1}, E_{t m_2})
\]

Assuming independent method and error terms across methods:

\[
\mathrm{Cov}(X_{t m_1}, X_{t m_2}) \;=\; \sigma_{T_t}^2
\]

Hence the **convergent validity correlation** is:

\[
r(X_{t m_1}, X_{t m_2}) \;=\; \frac{\sigma_{T_t}^2}{\sqrt{\mathrm{Var}(X_{t m_1}) \, \mathrm{Var}(X_{t m_2})}}
\]

Because neither method nor error is shared, this correlation is **lower than** same-trait/same-method reliability but **greater than** correlations where neither trait nor method matches.

### Heterotrait–Heteromethod (Different Trait, Different Method)

For different traits \( t_1 \) and \( t_2 \), different methods \( m_1 \) and \( m_2 \):

\[
\begin{aligned}
X_{t_1 m_1} &= T_{t_1} + M_{m_1} + E_{t_1 m_1} \\
X_{t_2 m_2} &= T_{t_2} + M_{m_2} + E_{t_2 m_2}
\end{aligned}
\]

Assuming traits are designed to be conceptually independent and method/error components are uncorrelated across traits/methods:

\[
\mathrm{Cov}(X_{t_1 m_1}, X_{t_2 m_2}) \;\approx\; 0
\]

Thus, **HTHM correlations** should be **lowest**, supporting **discriminant validity**.

### Heterotrait–Monomethod (Different Trait, Same Method)

For different traits \( t_1 \), \( t_2 \) with the **same method** \( m \):

\[
\begin{aligned}
X_{t_1 m} &= T_{t_1} + M_{m} + E_{t_1 m} \\
X_{t_2 m} &= T_{t_2} + M_{m} + E_{t_2 m}
\end{aligned}
\]

Their covariance is:

\[
\mathrm{Cov}(X_{t_1 m}, X_{t_2 m}) \;=\; \mathrm{Cov}(T_{t_1}, T_{t_2}) \;+\; \sigma_{M_m}^2 \;+\; \mathrm{Cov}(E_{t_1 m}, E_{t_2 m})
\]

If traits are distinct and errors are uncorrelated, then:

\[
\mathrm{Cov}(X_{t_1 m}, X_{t_2 m}) \;\approx\; \sigma_{M_m}^2
\]

This shows how **shared method variance** can **inflate HTMM correlations**, sometimes making them larger than convergent validities—an empirical warning sign that **method effects** may be dominating.

---

## Example: Synthetic MTMM Matrix (Campbell & Fiske, 1959)

### Example: Idealized Pattern

Campbell and Fiske provide a synthetic MTMM example (often colorized in teaching materials) illustrating ideal patterns:

- **Blue diagonal:** High reliabilities (same trait, same method)  
- **Green cells:** Positive convergent validities (same trait, different methods)  
- **Off-diagonal cells:** Lower correlations reflecting discriminant validity  

**Key takeaways:**

- Reliability correlations are the strongest.  
- Convergent validity correlations are positive and meaningful.  
- HTHM correlations are weakest.  
- Trait effects dominate method effects.  
- Patterns are consistent across hetero-method blocks.

---

## Example: Empirical MTMM Application

### Example: Long, Wong, & Song (2004)

**Observed patterns (as described):**

- **Reliability diagonals (parenthetical values):**  
  Mostly high (e.g., ~0.77–0.78 and above), which is strong by psychological research standards.

- **Convergent validity diagonals (bold values):**  
  Values such as 0.28, 0.34, 0.37, 0.32, 0.20, and 0.34—positive and acceptable.

- **Ordering criterion:**  
  Reliabilities exceed validities, and validities exceed most HTHM correlations.

- **Trait vs. method dominance:**  
  Not fully satisfied. Some heterotrait–monomethod correlations (e.g., ~0.55, ~0.42) exceed convergent validities.

**Interpretation:**

- Elevated HTMM correlations suggest **common method variance**.
- This pattern is common in **individual differences research**, such as personality.
- Further refinement may include:
  - Improving measurement specificity  
  - Adding additional methods  
  - Explicitly modeling method factors  

---

## Practical Guidance: Using MTMM for Validation

### Designing an MTMM Study

- Aim for **at least two traits and two methods**.  
- Select traits that are theoretically distinct.  
- Use meaningfully different methods (e.g., self-report, observer ratings, behavioral tasks).

### Evaluating Results

Check for:

- High reliability diagonals  
- Positive convergent validity  
- Proper ordering of correlations (Reliability > Convergent > HTHM)  
- Trait dominance over method effects (Mono-trait/hetero-method > Hetero-trait/mono-method)  
- Consistent hetero-method patterns  

### When Full MTMM Is Not Feasible

- Partial MTMM designs can still be informative.  
- Theoretical expectations about correlation patterns remain critical.  
- Limitations should be documented and addressed in future research.

---

## Conclusion

The MTMM framework operationalizes **construct validation** by making visible the contributions of **traits**, **methods**, and **error**. Grounded in **critical multiplism**, it encourages researchers to vary what they can, strengthening both generalizability and theoretical clarity. Even modest MTMM designs provide a powerful, transparent approach to validation.

---

## References

Campbell, D. T., & Fiske, D. W. (1959).  
*Convergent and discriminant validation by the multitrait-multimethod matrix.*  
**Psychological Bulletin, 56**(2), 81–105.

Long, E. C., Wong, C. S., & Song, L. J. (2004).  
Empirical application of multitrait–multimethod analysis in personality research.  
(Referenced as discussed in the lecture transcript.)


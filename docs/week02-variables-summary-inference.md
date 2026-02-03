---
title: "Week 2 – Variable Classification, Summary Statistics, and Inferential Decision Rules"
description: "Variable types and measurement scales, core summary statistics, and hypothesis testing decision rules with worked examples."
authors: ["Daniel B. Altieri"]
date: "2026-01-27"
tags: ["variables","measurement","summary statistics","inference","decision rules"]
toc: true
---

# Week 2 – Variable Classification, Summary Statistics, and Inferential Decision Rules

> **TL;DR**: Classify variables first (categorical vs. numeric; nominal/ordinal/interval/ratio). Match methods to types: 2-group mean → **t‑test**; ≥3 groups → **ANOVA**; two numeric variables → **correlation/regression**; binary DV → **logistic**; two categoricals → **chi‑square**. Always check assumptions and report uncertainty (e.g., **95% CI**).

**See also:** [Week  · [MTMM](./mtmm-construct-validation.md variable must exhibit variation across cases. Classify variables first by type—**Qualitative (Categorical)** vs. **Quantitative (Numeric)**—and then by **scale of measurement**: Nominal, Ordinal, Interval, or Ratio. This classification guides appropriate statistical procedures.

- **Examples**:
  - Number of votes → Quantitative, Ratio (meaningful zero).
  - Highest degree achieved → Qualitative, Ordinal.
  - Men’s pants sizes → Quantitative, Ratio.
  - Women’s jeans sizes → Qualitative, Ordinal (labels; inconsistent numeric steps).
  - Language proficiency → Depends on instrument (numeric test score vs. categorical level).

## 2. Summary Statistics
**Key measures (plain text)**
- Mean (arithmetic average): \(\\bar{x} = \\frac{1}{n} \\sum x_i\)
- Median: middle value when ordered; for even \(n\), \(\text{median} = \\frac{x_{n/2} + x_{n/2+1}}{2}\)
- Sample variance: \(s^2 = \\sum (x_i - \\bar{x})^2 / (n - 1)\)
- Sample standard deviation: \(s = \\sqrt{s^2}\)
- Population variance: \(\\sigma^2 = \\sum (x_i - \\mu)^2 / n\)
- Skewness (Fisher–Pearson): \(g_1 = m_3 / s^3\), where \(m_3 = \\text{mean}((x - \\bar{x})^3)\)
- Excess kurtosis (Fisher): \(g_2 = m_4 / s^4 - 3\), where \(m_4 = \\text{mean}((x - \\bar{x})^4)\)

**Worked Example** (n = 200)
- Sample mean (\(\\bar{x\)) = 52.144
- Sample median = 51.411
- Sample variance (\(s^2\)) = 145.968
- Sample std. dev. (\(s\)) = 12.082
- Skewness (\(g_1\)) ≈ 0.827
- Excess kurtosis (\(g_2\)) ≈ 1.340

**95% Confidence Interval for the mean (normal approximation)**
- \(\text{CI} = \\bar{x} \\pm z_{0.975} \\cdot SE(\\bar{x})\), where \(SE(\\bar{x}) = s/\\sqrt{n}\), \(z_{0.975} = 1.96\)
- Result: **[50.470, 53.819]**

## 3. Inferential Statistics & Decision Rules
Summary vs. inference: Summary statistics describe a sample; inferential methods test hypotheses and estimate parameters to generalize to populations.

**Hypothesis Testing Framework**
- **H0 (null)**: baseline claim (e.g., no difference)
- **H1 (alternative)**: competing claim
- **Test statistic**: function of data; compare to reference distribution
- **Decision rule**: Reject H0 if p-value ≤ α or if test statistic exceeds critical value

**Common procedures by scenario**
- Two-group mean comparison (DV quantitative, IV categorical with 2 levels): **independent-samples t-test**
- Multi-group mean comparison (DV quantitative, IV categorical with ≥3 levels): **ANOVA**
- Association between two quantitative variables: **Pearson correlation**; simple/multiple **linear regression**
- DV binary: **Logistic regression**; association between categorical variables: **Chi-square test**

**Worked Example: Choosing a Test**
- Scenario: Compare average training scores (numeric) between two departments (categorical: A vs. B).
- Classification → DV quantitative, IV categorical (2 levels) ⇒ independent-samples t-test.
- Decision rule (α = 0.05): reject H0 if t > t_crit or p-value ≤ 0.05.

## 4. Practical Guidance
- Focus on conceptual correctness: choose procedures that match variable type and scale.
- Checklist: confirm variables, identify scales, specify DV/IV, choose test via decision rules, inspect assumptions (normality, homoscedasticity, independence).

## FAQ

**Q: Are Likert scales ordinal or interval?**  
**A:** Strictly **ordinal** (ordered categories). Many analyses treat aggregated multi‑item Likert scales as approximately **interval**; justify and check robustness.

**Q: When do I choose ANOVA over multiple t‑tests?**  
**A:** When comparing **≥3 groups** to control **Type I error** and assess overall group differences before any post‑hoc comparisons.

**Q: What if normality or equal variances assumptions are violated?**  
**A:** Consider transformations, robust tests (e.g., Welch’s t/ANOVA), nonparametric alternatives (Mann‑Whitney, Kruskal‑Wallis), or bootstrap CIs.

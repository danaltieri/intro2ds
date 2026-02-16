# Student Guide: Creating Pivot Tables and Histograms in Excel

**Using the GSS\_2002\_multitrait\_labels Dataset**

***

## Learning Objectives

By the end of this lesson, students will be able to:

*   Understand the structure of a real-world survey dataset
*   Create pivot tables to summarize categorical data
*   Interpret pivot table outputs
*   Create and customize a histogram for numeric data
*   Choose the correct visualization for different data types

***

## Dataset Overview

**File:** `GSS_2002_multitrait_labels.xlsx`

*   Each row represents **one survey respondent**
*   Each column represents a **survey variable**, including:
    *   **happy** – self-reported happiness (categorical)
    *   **satjob** – job satisfaction (categorical)
    *   **Empathy** – numeric summary score
    *   **mntlhlth** – number of poor mental health days

⚠️ Some cells contain non-response codes:

*   `.i` = Inapplicable
*   `.d` = Do not know / Cannot choose

Non-numeric values must be handled before numeric analysis. One approach is filtering them out; another is manually sorting and removing them.

***

## Part 1: Preparing the Data

### Step 1: Open the File

1.  Open **Excel**
2.  Open `GSS_2002_multitrait_labels.xlsx`
3.  Select the worksheet containing the main data

**Visual description:**  
An Excel worksheet is visible, showing many rows of survey responses and column headers with variable names.

***

### Step 2: Turn On Filters

1.  Click any cell inside the dataset
2.  Go to **Data → Filter**

✅ Dropdown arrows appear in each column header.

**Visual description:**  
Column headers now include small filter dropdown arrows indicating filtering is enabled.

***

### Step 3: Filter Out Invalid Responses

For each variable you plan to analyze:

1.  Click the column’s filter arrow
2.  Uncheck:
    *   `.i: Inapplicable`
    *   `.d: Do not Know / Cannot Choose`
3.  Click **OK**

**Visual description:**  
A filter menu is open for a column, showing a list of values with `.i` and `.d` unchecked.

***

## Part 2: Creating a Pivot Table

### What Is a Pivot Table?

A **pivot table** summarizes large datasets by counting, averaging, or grouping values.

***

### Example 1: Count Respondents by Happiness Level

#### Step 4: Insert a Pivot Table

1.  Click inside the dataset
2.  Press **Ctrl + A** to select all data
3.  Go to **Insert → PivotTable**
4.  Choose **New Worksheet**
5.  Click **OK**

**Visual description:**  
The “Create PivotTable” dialog box shows a selected data range and the option to place the pivot table in a new worksheet.

***

#### Step 5: Build the Pivot Table

In the **PivotTable Fields** panel:

*   Drag **happy** → **Rows**
*   Drag **id\_** → **Values**

Excel defaults to **Count of id\_**.

**Visual description:**  
The PivotTable Fields panel shows *happy* in Rows and *Count of id\_* in Values, with a summary table appearing in the worksheet.

***

#### Step 6: Interpret the Pivot Table

You should see:

*   **Rows:** Happiness categories
*   **Values:** Number of respondents in each category

This answers the question:

> **How many people report each level of happiness?**

**Visual description:**  
A pivot table lists happiness levels (e.g., VERY HAPPY, PRETTY HAPPY) with corresponding counts and a grand total.

***

## Part 3: Expanding Pivot Table Analysis

### Example 2: Happiness by Job Satisfaction

1.  Keep **happy** in **Rows**
2.  Drag **satjob** → **Columns**
3.  Keep **id\_** → **Values (Count)**

This creates a two-way table showing how happiness varies by job satisfaction.

**Visual description:**  
A pivot table displays happiness levels as rows and job satisfaction categories as columns, with counts in each cell and totals.

***

## Part 4: Creating a Histogram

### What Is a Histogram?

A **histogram** shows the **distribution of a numeric variable** by grouping values into ranges (bins).

⚠️ Histograms require **numeric data only**.

Good candidates in this dataset:

*   **Empathy**
*   **mntlhlth**

***

### Example: Distribution of Empathy Scores

#### Step 1: Select and Prepare the Data

1.  Select the entire **Empathy** column
2.  Apply a filter if needed
3.  Remove any non-numeric values

**Visual description:**  
The Empathy column is highlighted, with a filter menu showing only numeric values selected.

***

#### Step 2: Insert the Histogram

1.  With the numeric column selected, go to **Insert**
2.  Click **Insert Statistic Chart**
3.  Choose **Histogram**

Excel automatically generates the histogram.

**Visual description:**  
The Excel chart menu is open, and a histogram chart appears showing bars representing empathy score ranges.

***

#### Step 3: Customize the Histogram

1.  Click the horizontal axis
2.  Right-click → **Format Axis**
3.  Adjust:
    *   **Bin width** (e.g., 0.5 or 1)
    *   **Number of bins**
4.  Add titles:
    *   **Chart Title:** *Distribution of Empathy Scores*
    *   **X-axis:** *Empathy Score*
    *   **Y-axis:** *Number of Respondents*

**Visual description:**  
A histogram is shown with labeled axes, and the Format Axis panel is open with bin options visible.

***

## Key Takeaways for Pivot Tables and Histograms

### Choosing the Right Tool

| Data Type          | Tool        |
| ------------------ | ----------- |
| Categorical        | Pivot Table |
| Numeric            | Histogram   |
| Group comparisons  | Pivot Table |
| Distribution shape | Histogram   |

***

### Common Mistakes

❌ Including `.i` or `.d` values  
❌ Using histograms for categorical data  
❌ Missing chart labels

✅ Always clean data first and label visuals clearly.

***

### Reflection Questions

*   What does the empathy distribution tell you?
*   How does job satisfaction relate to happiness?
*   Why is a histogram appropriate for empathy scores?

***


# Week 7 Live Class Meeting summary

### Key takeaways
- Regression analysis is a fundamental predictive tool, but has limitations when assuming linearity
- Understanding regression helps identify gaps in machine learning models like LLMs
- Data variance is essential for meaningful analysis - without variance, there's no predictive value
- Common mistakes in regression are not in calculation but in selecting the wrong explanatory variables
- Exploratory Data Analysis (EDA) is both a philosophy and starting point for any data analysis
- Python offers more efficient tools for data analysis compared to Excel

## Discussed topics

### Linear vs. Non-linear Regression Models
Discussion on the limitations of linear regression and the traps of assuming linearity in complex systems.

**Details**
- **Daniel**: Explained how regression is fundamental to understanding gaps in machine learning models like ChatGPT
- **Charlotte**: Noted that "correlation does not mean causation"
- **Pitts**: Mentioned that regression tries to get a line to intersect as many points as possible
- **E.J.**: Observed that models try to represent what is and predict what might be, but can't perfectly replicate contributing factors
- **Daniel**: Confirmed that models take known information to predict unknowns with only partial information

**Conclusion**
- Linear models often fail to predict significant changes or "hockey stick" patterns
- Models are simplifications of complex realities with inherent limitations
- Real-world examples often don't follow linear patterns (learning curves, consumption patterns)

### Data Variance and Its Importance
Discussion on why variance is crucial for data analysis and predictive modeling.

**Details**
- **Daniel**: Posed the question about what variance helps determine
- **Jonathan**: Answered that variance shows how diverse a data set is
- **Jany**: Shared a work example where survey data with little variance (all 9s and 10s) wasn't useful for analysis
- **Daniel**: Explained that without variance, there's no difference to analyze between observations

**Conclusion**
- Variance is necessary to determine differences between observations
- Without variance, there's no predictive value in the data
- Even lack of variance can be informative in certain contexts

### Multi-collinearity in Data Analysis
Explanation of when variables are too closely related to provide distinct predictive value.

**Details**
- **Daniel**: Provided an example from corporate learning where satisfaction and relevance measurements were highly correlated
- **Joe**: Had previously asked about multi-collinearity

**Conclusion**
- Multi-collinearity occurs when two variables essentially measure the same thing
- Using collinear variables doesn't add unique predictive value to models

### Data Leakage in Model Training
Discussion on how models can be contaminated to appear more predictive than they actually are.

**Details**
- **Daniel**: Compared data leakage to cheating on tests, where the model has access to information it shouldn't
- **Jany**: Suggested that removing data or having too much missing data could affect models

**Conclusion**
- Data leakage occurs when models are trained with information that wouldn't be available in real-world prediction scenarios
- Survey design can create data leakage if questions telegraph what researchers are looking for
- Manipulating training data can artificially improve model performance

### Action Research vs. Existing Data Sets
Discussion on the practical aspects of collecting data in workplace environments.

**Details**
- **Adrienne**: Explained that action research might be more accessible in workplaces due to permission issues with existing data
- **Adrienne**: Noted that action research involves defining user groups, parameters, and research questions, then collecting data directly

**Conclusion**
- Action research can be more practical in workplace settings where access to existing data is limited
- Creating and collecting your own data provides more agency but may be smaller in scale

### Exploratory Data Analysis (EDA)
Discussion on the importance and application of EDA as both a philosophy and tool.

**Details**
- **Daniel**: Emphasized that EDA is a philosophy and starting point for any data collection
- **Daniel**: Noted that even small datasets benefit from some level of exploratory analysis

**Conclusion**
- EDA should be applied to all data, though the depth may vary based on dataset size
- Understanding variance through EDA is crucial for determining what information exists in the data

### Excel vs. Python for Data Analysis
Demonstration of how Python can perform the same analyses as Excel but more efficiently.

**Details**
- **Daniel**: Demonstrated how to perform various analyses in Python using Colab
- **Evan**: Expressed appreciation for seeing Python as an alternative to Excel
- **Pitts**: Mentioned his fondness for Excel, particularly VBA for engineering applications

**Conclusion**
- Python offers more streamlined methods for statistical analysis and visualization
- Both tools have their place depending on user preference and specific needs
- Colab provides an accessible environment for Python-based data analysis

## Action items

### All students
- Complete the exploratory data analysis exercises if not finished during class
- Consider using the shared Colab notebook to explore Python-based data analysis
- Review the Excel Data Miner toolpack installation instructions

### Daniel
- Share additional examples of data leakage in follow-up email
- Provide instructions on how to get the Data Miner toolpack for Excel
- Find and potentially share the HBR supply chain exercise mentioned in class

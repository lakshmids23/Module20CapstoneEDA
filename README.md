# Exploratory Data Analysis on NHANES 2013–2014: Deriving a Mental Health Binary Indicator

## Executive Summary
This project leverages **NHANES 2013–2014 data** to derive a composite mental health score from questionnaire items analogous to the **PHQ-9**. By converting this continuous score into a binary indicator for clinically significant depressive symptoms, the analysis explores patterns and associations between mental health status, dietary intake, and demographic characteristics. The project uses robust data cleaning, merging, visualization, and statistical testing to uncover insights that can inform targeted healthcare interventions.

## Rationale
**Depressive disorders** represent a major public health challenge, impacting quality of life and increasing healthcare costs. Accurately identifying individuals with clinically significant depressive symptoms is crucial for early intervention, efficient resource allocation, and designing tailored treatment strategies. This analysis offers a data-driven approach to understanding mental health trends in a nationally representative dataset, providing actionable insights for healthcare decision-makers.

## Research Question
Can we effectively classify U.S. adults’ depressive symptomatology using a composite mental health score derived from **NHANES 2013–2014 data**, and what are the key associations between this binary mental health indicator and dietary and demographic factors?

## Data Sources
- **Questionnaire Data:** NHANES 2013–2014 mental health items (**DPQ variables**) used to compute the composite mental health score.  
- **Dietary Data:** First-day 24-hour dietary recall data capturing nutrient intakes, including macronutrients and micronutrients.  
- **Demographic Data:** Participant characteristics such as **age**, **gender**, **race/ethnicity**, **education**, **income-to-poverty ratio**, **marital status**, **household size**, and **nativity**.  

## Methodology
1. **Data Integration:** Merging multiple datasets (questionnaire, dietary, and demographic) using a unique participant identifier.  
2. **Data Cleaning & Preparation:** Handling missing values via imputation (median for numerical, mode for categorical), recoding specific values, and de-duplication.  
3. **Composite Score Development:** Summing mental health-related items (**DPQ variables**) to create a continuous score and converting it into a binary variable using a clinically validated cutoff of **10**.  
4. **Exploratory Data Analysis:** Conducting univariate, bivariate, and multivariate visualizations (**histograms, box plots, correlation heatmaps, and pair plots**) to explore distributions and relationships.  
5. **Statistical Testing:** Employing **t-tests** and **non-parametric tests (Mann-Whitney U)** to assess differences between groups, and computing **correlation matrices** to evaluate associations among continuous variables.  

## Results
- **Mental Health Classification:** Approximately **6%** of the sample were identified as having clinically significant depressive symptoms based on the binary indicator.  
- **Dietary & Demographic Insights:** Analysis showed largely overlapping distributions of nutrient intakes between mental health groups. While some slight trends were observed (e.g., marginal differences in energy intake and certain nutrient distributions), statistical tests suggested that differences were borderline or non-significant.  
- **Correlation Analysis:** Strong correlations were found among related dietary measures (e.g., total fat and saturated fat) and between total energy intake and its macronutrient components, highlighting the robustness of the underlying dietary data.  

## Next Steps
- **Refine Predictive Models:** Develop advanced classification models (e.g., logistic regression, ensemble methods) to predict mental health status.  
- **Subgroup Analysis:** Explore the influence of additional covariates such as socioeconomic status and lifestyle factors in more detail.  
- **External Validation:** Compare findings with other cycles of NHANES or external datasets to validate the clinical cutoff and predictive performance.  
- **Longitudinal Analysis:** Consider temporal trends or causal inferences with additional cycles of data collection.

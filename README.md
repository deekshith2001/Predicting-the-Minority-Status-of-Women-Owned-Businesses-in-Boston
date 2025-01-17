# Predicting the Minority Status of Women-Owned Businesses in Boston

## Overview
This project leverages machine learning to predict the minority status of women-owned businesses in Boston by analyzing geographic, socioeconomic, and business-type data. The primary objective is to provide actionable insights to policymakers, enabling equitable resource allocation and fostering economic growth among minority women entrepreneurs.

---

## Background
Women-owned businesses, particularly those led by minority women, face systemic challenges such as:
- Lower survival rates compared to male-owned businesses.
- Limited financial resources.
- Spatial and economic barriers that restrict their growth.

This project addresses these disparities by developing predictive tools to identify businesses that may benefit from targeted support, enhancing socioeconomic equity and business sustainability.

---

## Objectives
1. **Prediction**: Classify women-owned businesses as minority-owned or non-minority-owned based on their geographic location, business type, and the socioeconomic status of their surrounding area.
2. **Insight Generation**: Provide data-driven insights to support equitable resource distribution and promote sustainability for minority women-owned businesses.

---

## Data Sources
1. **Women-Owned Businesses**:  
   - Provided by the Boston city government.
   - Contains data on business type, location, and demographic attributes.
2. **Median Income Data**:  
   - U.S. Census Bureau's American Community Survey (2021).
   - Median income data by census tract in the Greater Boston area.

---

## Methodology
### Data Preparation
- **Geocoding**: Business addresses were geocoded to obtain coordinates for spatial analysis.
- **Categorization**: Business types were grouped into nine categories to simplify modeling.
- **Data Merging**: Census data was spatially joined with geocoded business data for socioeconomic insights.

### Machine Learning Models
1. **k-Nearest Neighbors (kNN)**:
   - Assumes that businesses in similar locations have similar demographic characteristics.
   - Achieved the highest accuracy at 71.1%.
2. **Random Forest**:
   - Evaluates variable importance through binary splits.
   - Highlighted the significance of median income and proximity to Boston.
3. **Logistic Regression**:
   - Assesses statistical significance and the effect of variables.
   - Forward selection achieved an accuracy of 65.4%.

---

## Key Findings
- **Location and Income**: Median income and distance from Boston are the most significant predictors of minority business ownership.
- **Business Type**: Business type did not significantly enhance model accuracy.
- **Policy Implications**: Policymakers can use these insights to direct resources toward areas of lower socioeconomic status to promote equity and business growth.

---

## Limitations
1. Small dataset (195 businesses) limits generalizability.
2. No disaggregated data by race or ethnicity.
3. Focused only on women-owned businesses in Boston; findings may not apply to other cities.
4. Limited availability of continuous variables in the dataset.

---

## Future Work
- Expand the dataset to include additional cities and demographic data.
- Incorporate advanced machine learning techniques for improved accuracy.
- Analyze gender and race intersections to uncover deeper insights.
- Continuously update the model with new data to enhance predictive capabilities.

---

## Repository Structure
- **data/**: Contains raw and processed datasets.
- **notebooks/**: Jupyter notebooks for exploratory data analysis and model development.
- **results/**: Outputs and visualizations from the analyses.
- **src/**: Python scripts for data preprocessing, modeling, and evaluation.
- **README.md**: Project documentation.

---

## Acknowledgments
This project was completed as part of the DATA 200 course at Tufts University. Special thanks to our team members:
- Arlyss Herzig
- Anushka Pandey
- Marco Hong
- Deekshith Komira

---

## References
1. Robb, Alicia M. "Entrepreneurial Performance by Women and Minorities: The Case of New Firms." *Journal of Developmental Entrepreneurship*, 2002.
2. U.S. Census Bureau. "Median Income in the Past 12 Months." *American Community Survey*, 2021.
3. Data provided by the Boston City Government.

---

Thank you for exploring this project! For any inquiries, please feel free to [contact us](mailto:your-email@example.com).

# Concrete Strength Prediction and Analysis

## Project Overview
This project aims to analyze the impact of different concrete compositions and curing times on compressive strength using a combination of exploratory data analysis, hypothesis testing, and regression modeling. Concrete strength is a critical factor in construction, and understanding how different components (such as cement, water, fly ash, etc.) influence this property is essential for optimizing concrete mix designs.

The project explores relationships between concrete components and strength, tests hypotheses about differences in strength based on water levels and concrete age, and builds a predictive model to estimate concrete strength from its components. This analysis provides actionable insights that can help construction companies design more durable and cost-effective concrete mixes.

# Technologies Used
R: Programming language for data analysis
Packages:
- tidyverse: for data manipulation (dplyr), visualization (ggplot2), and more.
- corrplot: for visual representation of correlation matrices using correlation plots.
- readxl: for importing Excel files into R easier.
- datarium: for some statistical analysis.
- qqplotr: for creation of quantile-quantile (Q-Q) plots for testing normality.
- rcompanion: for statistical analysis e.g for nonparametric tests.
- lattice: for creating multi-panel plots for visualizing data.
- car: for regression and hypothesis testing.
- FSA: functions for statistical testing.
- RVAideMemoire: for statistics and model, and nonparametric tests.

## How to Run
To replicate this project:

1 Clone this repository:
```bash
git clone https:/github.com/B-Taiwo/concrete-strength-statistical-analysis.git
```
2. Install dependencies: Ensure you have R installed on your machine. Then, use the following R command to install the necessary packages:
```r
install.packages(c("tidyverse", "corrplot", "readxl", "datarium", 
                   "qqplotr", "rcompanion", "lattice", "car", 
                   "FSA", "multcomp", "RVAideMemoire"))
```
3. Run the provided .Rmd (R Markdown) file `concrete analysis.Rmd` in RStudio to see the full analysis and results.

4. View the final report: The final report in the directory can be viewed in PDF format `concrete analysis.pdf`.

## Project Results
### Summary of Findings
The aim of this report was to analyze how compressive strength in concrete is influenced by its 
composition and provide actionable insights for the construction company. The key findings include:
1. Curing Time (Age): Compressive strength increases significantly with curing time. Strength 
differences were clear across Early, Standard, and Mature Age groups, confirming that 
extended curing time leads to higher concrete strength. This highlights the importance of 
ensuring sufficient curing periods to achieve desired strength levels.
2. Water Content: Water content strongly affects compressive strength, with Low water levels 
producing significantly higher strength than Middle or High water levels. This shows the critical 
role of water-cement ratios in concrete design and the need to minimize excess water.
3. Fly Ash and Particle Size: Neither the presence of fly ash nor the Fine vs. Coarse particle size 
categories significantly impacted compressive strength.
4. Regression Models:
- Regression analysis identified Cement, Water, Blast Furnace Slag, and Fly Ash as 
significant predictors of compressive strength. Water content had the strongest 
negative effect, while Cement and supplementary materials (slag and fly ash) 
contributed positively.
- The best regression model explained 44% of the variability in compressive strength.

### Practical Implications and Conclusion 
The company should prioritize controlling water content and optimizing curing times to maximize 
compressive strength. Cement, slag, and fly ash can be adjusted strategically without compromising 
strength. The results are in line with industry standards, giving the construction company suggestions 
based on data to improve performance by adjusting mix ratios and curing times.

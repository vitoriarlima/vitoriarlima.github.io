---
title: "PCA on a Bonds Portfolio"
excerpt: "An analysis and literature review of factor investing in fixed income, where the first three components can be attributed to actual meanings in a Bonds Portfolio setting."
collection: portfolio
---

# Principal Component Analysis of the Term Structure of European Interest Rate Yields

## Overview

This project explores the application of Principal Component Analysis (PCA) to the term structure of European interest rate yields over the period from 2004 to 2020. The dataset includes daily interest rate yields of AAA-rated bonds from various maturities, spanning from one year to thirty years. The primary aim is to investigate the efficacy of PCA in identifying the main factors that drive changes in the yield curve, especially in different interest rate environments.

### Key Objectives

1. **PCA Application**: Apply PCA to the term structure of interest rate yields to identify the primary components that explain the variability in the yield curve.
2. **Shift, Slope, and Curvature**: Interpret the first three principal components (PCs) as shift (or level), slope (or steepness), and curvature of the yield curve, respectively.
3. **Interest Rate Environment Analysis**: Compare the efficacy of PCA in positive and negative interest rate environments, evaluating whether the amount of variability explained by the first three PCs differs between these environments.

### Methodology

- **Data Collection**: The dataset comprises daily yield data for AAA-rated bonds in the Euro Area, sourced from the Eurostat Database. The time series spans from September 6, 2004, to September 23, 2020.
- **Data Partitioning**: The data is divided into five parts for detailed analysis:
  1. **Part 1**: Entire dataset (2004-2020)
  2. **Part 2**: Positive interest rate environment (2004-2007)
  3. **Part 3**: Negative interest rate environment (2014-2017)
  4. **Part 4**: Deep negative interest rate environment (2017-2020)
  5. **Part 5**: Extended negative interest rate period (2014-2020)
- **Stationarity**: Ensuring stationarity of the data by taking the first differences of the yields.
- **PCA Implementation**: Conduct PCA on the correlation matrix of the first differences of the yield data to identify the principal components.

### Findings

- **Shift, Slope, and Curvature**: The first three PCs effectively represent the shift, slope, and curvature of the yield curve, consistent with findings in previous literature.
- **Interest Rate Environment**: Contrary to some recent studies, this analysis finds no significant difference in the efficacy of PCA between positive and negative interest rate environments. The amount of variability explained by the first three PCs remains substantial in both cases.

### Conclusion

This project demonstrates the robustness of PCA in analyzing the term structure of interest rates. The findings suggest that PCA can reliably capture the main factors driving yield curve changes across different interest rate environments. These insights are valuable for risk management and portfolio optimization in the bond market.

---

### Repository and Resources

For more details and access to the code, please visit the [GitHub Repository](https://github.com/vitoriarlima/pca-bonds-fixed-income).

To read the full analysis, you can download the [PDF file](https://vitoriarlima.github.io/files/PCA_Bond_Portfolio.pdf).


---

### Pretty Visualizations

![Bond Maturities over time](/Users/vitorialima/Desktop/personal/personal website/vitoriarlima.github.io-/files/Bond maturities over time.png)

![Time Path of the Term Structure](/Users/vitorialima/Desktop/personal/personal website/vitoriarlima.github.io-/files/Time path of the term structure.png)

![Yield Curves from AAA rate bonds in the european area](/Users/vitorialima/Desktop/personal/personal website/vitoriarlima.github.io-/files/Yield curves from AAA-rated bonds in the european area.png)

### Overview

This project, **ACTL2111 Probability & Mathematical Statistics (Individual Assignment 1)**, used a Monte Carlo simulation to model an auto insurance pool. The goal was to analyze the statistical properties of pooled risks and calculate a minimum premium to ensure financial solvency. The model was built to be easily adjusted for key parameters, demonstrating a flexible and reusable approach. For more details, refer to [the project webpage](https://quenstance.pages.dev/projects/auto-insurance-monte-carlo-simulation/).

### How to Use

The simulation was built in Microsoft Excel. The spreadsheet allows users to adjust key parameters:
* Number of drivers (**n**)
* Individual probability of accident (**p**)
* Average size of accident (**beta**)
* Histogram bin minimum and bin interval
* Probability of sufficiency

All calculations and results will automatically update based on the new parameters.

### Methodology

The simulation ran for an accident year with **1,000 drivers**. The number of claims and their costs were simulated using Excel's `RAND()` function, leveraging the property that the sum of independent exponential random variables follows a **Gamma distribution**. Key metrics, including mean and standard deviation of total claims cost and the average cost per policyholder, were calculated using `AVERAGE`, `STDEV.S`, and `PERCENTILE` functions to derive the minimum premium.

### Limitations

* **Tool**: The use of Excel's `RAND()` function is a key limitation, as its volatile nature makes results difficult to reproduce consistently. For larger-scale simulations, professional tools like Python or R are superior due to their performance and reproducibility.
* **Model Assumptions**: The model uses static parameters and simplifies real-world conditions by assuming claims are independent and follow a perfect exponential distribution. While a reasonable academic assumption, real-world data may exhibit dependencies, which could affect the accuracy of the final premium calculation.

### Author

**Quenstance Lau**
* **Web Portfolio**: https://quenstance.pages.dev/
* **LinkedIn**: https://www.linkedin.com/in/quenstance/
* **GitHub**: https://github.com/quenstance

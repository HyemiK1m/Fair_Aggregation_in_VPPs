# Fair Aggregation in Virtual Power Plants

This repository contains the source code to reproduce the findings presented in the research paper titled **"Fair Aggregation in Virtual Power Plants"**. Please refer to the [full paper](link) for more details.

## Experimental Setup
Most scripts in this repository utilize the **Pyomo** library to solve optimization problems. While the codebase is tailored for use with **Google Colab**, it can also be executed locally by installing the necessary dependencies and solvers (e.g., Pyomo, Ipopt, or Couenne).

## Stylized Model and Multiple Consumer Cases
Results for different fairness criteria (**Energy, Price, and Utility**) based on the stylized model and 3-consumer cases can be found in the `Stylized_Model` folder:
* `Energy_Fairness.ipynb`
* `Price_Fairness.ipynb`
* `Utility_Fairness.ipynb`

## Case Study
All relevant files are located in the `Case_Study` folder. To reproduce the results in Section 5, please follow these steps:

1. **Download Data**: Download the iFlex dataset from [Zenodo](https://zenodo.org/records/8248802).
2. **Preprocessing**: Run `data_analysis.ipynb` to preprocess the data.
3. **Run Experiments**: Using the parameters estimated from the preprocessing step, run the following files to get the results:
   * `Energy_Fairness.ipynb`
   * `Price_Fairness.ipynb`
   * `Utility_Fairness.ipynb`
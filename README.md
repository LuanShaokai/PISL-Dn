Symbolic Regression for Newmark Displacement and Seismic Parameters Relationship
This repository contains Python code for establishing a relationship between Newmark displacement and seismic parameters using symbolic regression with STRidge algorithm.
Core Features
	STRidge Algorithm: Implements the Sequential Threshold Ridge Regression (STRidge) algorithm to find sparse approximations and establish the relationship between Newmark displacement and seismic parameters.
	Customizable Function Library: Allows users to define a function library including various mathematical operations on seismic parameters to explore different feature combinations.
	Evaluation Metrics: Provides multiple evaluation metrics such as MSE, MAE, RMSE, MAPE, R, and R² to assess the performance of the established relationship.
Installation
	Python Version: Python 3.9
Required Libraries:
	Library	Purpose
	numpy	Numerical operations
	pandas	Data manipulation
	sklearn	Machine learning metrics
	matplotlib	Plotting (optional)
	sympy	Symbolic mathematics
	scipy	Scientific computing
Usage
	Prepare Your Data: Ensure your seismic data is in a compatible format (e.g., Excel file) with columns representing different seismic parameters (logIa, ac, c, acbpga, Ia, etc.) and the target Newmark displacement (logDn).
	Modify the Main Code:
	 Update the file path in pd.read_excel() to point to your data file.
	 Adjust the func_dict list to define your desired function library based on your seismic parameters.
	 Set hyperparameters such as lam, tol, iters according to your needs.
	Run the Code: Execute the script to perform symbolic regression and establish the relationship. The code will output the evaluation metrics and save the results.
Data Description
	The dataset provided in this repository includes seismic records from the Wenchuan, Ludian, and Lushan earthquakes. It contains four levels of critical acceleration (ac): 0.2g, 0.15g, 0.1g, and 0.05g.
	Due to data confidentiality requirements, only the seismic ground motion parameters are provided — the station codes and exact locations are not disclosed..
Example Output
	The code will generate an equation representing the relationship between Newmark displacement and seismic parameters. It will also output evaluation metrics to assess the performance of the established relationship. Additionally, the true and predicted values will be saved in a text file for further analysis.
Note
	Feel free to modify and extend the code to suit your specific research or application needs. If you encounter any issues or have suggestions for improvement, please feel free to contact the repository owner.

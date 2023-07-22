# large_ds_management_r
Wrangling 4.6M Rows (375MB) in R.
Data Wrangling Tools by Dataset Size

# Findings
- Both DT & dplyr great for data manipulation
- DT is faster on grouped mutations (). Speedup of 2X-10X on inplace calculations using := 
- DT can be slower than dplyr on grouped summarizations

- `dplyr` (1M Rows+)
- `data.table` (10-50M Rows+)
- `Spark / sparklyr` (100M Rows+)

### Business Objectives
Loan defaults cost organizations multi-millions -> Need to understand which people or institutions will default on loans.

### Dataset
https://loanperformancedata.fanniemae.com/lppub/index.html


### To run the script 
1. Download the dataset;
2. Put the data into `./data` folder
3. Restore env by running `renv::restore(lockfile = 'renv.lock')`
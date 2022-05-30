### module_14_challenge
files and analysis for module 14 challenge

baseline plot
![Image](/actual_vs_strategy_basline.png)


### Step 6: Use an Alternative ML Model and Evaluate Strategy Returns
In this section, you’ll tune, or adjust, the model’s input features to find the parameters that result in the best trading outcomes. You’ll choose the best by comparing the cumulative products of the strategy returns.



## Step 1: Tune the training algorithm by adjusting the size of the training dataset. 
To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your `README.md` file. 

Answer the following question: What impact resulted from increasing or decreasing the training window?

increasing the training window made the two plots more closely align

![Image](/actual_vs_strategy_12mo_shift.png)

## Step 2: Tune the trading algorithm by adjusting the SMA input features. 
Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your `README.md` file. 

Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?

decreasing both SMA windows to 3 and 30 respectively had a positive impact on the strategy causing it to outperform the actual returns

![Image](/actual_vs_strategy_3and30sma.png)

## Step 3: Choose the set of parameters that best improved the trading algorithm returns. 
Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your `README.md` file.

leaving the training window at 3 months but changing the SMA to 3 and 30 days caused both or the ML trading algorithms to outperform the actual returns during this period.

![Image](/logisticreg_3and30sma.png)
![Image](/actual_vs_strategy_3and30sma.png)
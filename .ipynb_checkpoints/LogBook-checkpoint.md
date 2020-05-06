Here are the steps we took:
1. Run regresssion with all default parameters from the Boston housing price example. Results were generally comparable to random forest. Runtime was around 10 mins for each. Precip plot showed signs of large overfitting! 1000 epochs was more than enough.
2. Focused on precip overfitting: Reduced complexity of the model significantly: now only 1 hidden layer with 4 nodes. Also looked at early stopping based on MSE but no improvement.
3. For other models I increased complexity to 2x 64-node hidden layers but result was worse. So far best results for wind & temp is with MSEProp optimizer with one hidden layer of 20 neurons!
4. The theme seems to be that the proposed tactic of 1) making the model overly complex to induce overfitting and then 2) introducing checks & balances to find the sweet spot... did not work. The best results so far seem to be from ensemble methods but with very simple models - just one layer and changing the number of units. 

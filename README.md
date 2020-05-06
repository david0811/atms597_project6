# ATMS 597 Project 6 Group D
## Group Members: Sarah Szymborski, Michael Sessa, David Lafferty
<b>Problem:</b><br>
Use a neural network to predict 4 daily weather variables for Champaign, IL: maximum temperature, minimum temperature, maximum wind speed, and total precipitation. We use 2010-2018 for training data and 2019 for testing. We evaluate the model against a pre-optimized random forest algorithm using root mean square error (RMSE) as a metric.

<b>Notebooks:</b>
- `BaselineModels`: Runs the random forest baseline as well as the neural network models with a minimum of 3 layers.
- `NeuralNetEnsemble`: Based analyzing results from the 3-layer neural networks, we implemented an emsemble method in order to improve scores. We build a 26-member ensemble of 1-layer neural networks with 4-30 neurons in the layer for each target variable. This ultimately provides our lowest RMSE values.

<b>Results:</b><br>
(All results are RMSE for test data)<br>
Maximum Temperature: 1.87$^\circ C$<br>
Minimum Temperature: 1.99$^\circ C$<br>
Maximum Wind Speed: 1.58$m/s$<br>
Total Precipitation: 4.17$mm$<br>
<br>
Our presentations slideshow can be found [here](https://docs.google.com/presentation/d/1Vbn-lfG2Pqav0wvZa_5e79oAYcXZHLiSHAU5CfN6mOI/edit?usp=sharing)
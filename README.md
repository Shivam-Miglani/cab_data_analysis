# Cab Spotting Data Challenge by PMI

My solution lies in the `notebooks` folder. It contains 4 notebooks:

1. `00_EDA_preprocessing.ipynb`: The notebook states the business objectives and contains basic EDA and preprocessing of dataset.
   1. Notebook plots interactive temporal heatmaps to visualize cabtrails throughout the time period
   2. Notebook plots fraction of empty cabs
2. `01_CO2_reduction.ipynb`: The notebook explores the first task of estimating yearly CO2 emission reduction caused due to unoccupied cabs.
   1. The notebook explores how to calculate the `distance` between two coordinates
   2. Does more advanced EDA with trip duration and distances, ultimately finds and removes outliers
   3. States assumptions made and calculates the potential CO2 estimates (wheel and well-to-wheel estimates).
3. `02_passenger_prediction.ipynb`: Notebook takes the processed data and builds a model for taxi drivers to predict location of next passengers.
   1. Feature Engineering
      - time-based, location based and previous trip based features
   2. Very fast hist gradient boosting model, which can even be used for online training to do live predictions!
   3. Prediction example
   4. MLOps demonstration
4. (Bonus) `03_cab_clusters.ipynb`: This notebook attempts to find cab clusters using ML and domain knowledge.
   1. Uses advanced geoplotting to visualize the solution (notebook 0.)
   2. Segregates profit-making, under-utilized, efficient and liability drivers




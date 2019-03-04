Assignment 2 - Randomized Optimization - lhu81

Code: https://github.com/huhu42/assignment2

The code in this assignment implements three randomized optimization problems (TSP, FLIPFLOP and CONTPEAKS) as well as optimizing weights to the Neural Network implemented in Assignment 1 for credit card default. 

Data:

The data has been pre-processed and saved in the "Data" folder as "CreditDefaultData_train.csv","CreditDefaultData_test.csv" and "CreditDefaultData_validate.csv". 

Output:

Output CSVs and images are written to `./output` and `./output/images` respectively. Sub-folders will be created for
each toy problem (`CONTPEAKS`, `FLIPFLOP`, `TSP`) and the neural network from the _Supervised Learning Project_ (`NN_OUTPUT`, `NN`).

If these folders do not exist the experiments module will attempt to create them.

Running Experiments:

Each experiment can be run as a separate script. Running the actual optimization algorithms to generate data requires the use of Jython 2.7. 

For the neural network problem, run:
 - NN-Backprop.py
 - NN-GA.py
 - NN-RHC.py
 - NN-SA.py
 
 For the three randomized optimization problems, run:
 - continuouspeaks.py
 - flipflop.py
 - tsp.py

Graphing:

The `plotting.py` script takes care of all the plotting. Since the files output from the scripts above follow a common naming scheme it will determine the problem, algorithm, and parameters as needed and write the output to sub-folders in `./output/images`. This _must_ be run via python 3, specifically an install of python that has the requirements from `requirements.txt` installed.

In addition to the images, a csv file of the best parameters per problem/algorithm pair is written to`./output/best_results.csv`

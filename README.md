# Extended-preprocessing-LSH-eur

# Introduction
This code belongs to the paper "Extended pre-processing of LSH for Duplicate Detection". All the needed functions are included in the Jupyter Notebook file. It can be run by setting the os.chdir command to the right location (where the .json file is located) and then simply running the whole file.

# What is included?
- A .ipynb file containing all the code needed to run the duplicate detection algorithm
- A .json file cointaining the data of televisions from 4 different web shops.

# Description of code
The code contains the following parts:

Loading data:
Here we load the data 

Cleaning data:
Here we clean the data to increase similarity and make it easier to find duplicates

Find modelID:
Here we try to find the modelID used in the title.

Set dictionaries:
Here we create dictionaries for every product, with as key the index of the product and as value either the modelID, possible modelID, modelwords in title or shop name

Create brandlist:
Here we create a list of all brands included in the data set.

Signature matrix:
Here we create a signature matrix build from the binary vectors

LSH hashing:
We now use LSH to create buckets and decrease the needed number of comparisons

JacSim:
In the last phase we compute the jaccard similarty

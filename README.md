# Extended-preprocessing-LSH-eur

# Introduction
E-commerce is growing, resulting in more and more web
shops. As web shops often offer the same products but have a different
representation, it could be useful to detect duplicates among sites.
This paper provides a scalable method to detect duplicates of a data set
of televisions. By extensive pre-selection, the number of comparisons between
possible duplicates is reduced. This pre-selection consists of data
cleaning to create more similarity between products, extending important
data from the title of the product, and uses minhashing and LSH
to select possible pairs. The performance is analyzed using the F1 score
and it is found that the applied method has a significant increase in the
scalability of duplicate detection.

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


#Running the code
This code belongs to the paper "Extended pre-processing of LSH for Duplicate Detection". All the needed functions are included in the Jupyter Notebook file. It can be run by setting the os.chdir command to the right location (where the .json file is located) and then simply running the whole file.

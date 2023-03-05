# Cryptocurrencies

## Purpose

The purpose of this analysis was to use unsupervised machine learning to classify cryptocurrencies in order to provided an investment portfolio for customers of Accountability Accounting. 

## Results

Using a dataset from CryptoCompare (https://min-api.cryptocompare.com/data/all/coinlist), I read the .csv into a pandas Dataframe and transformed the data to get a view of all the tradable cryptocurrencies. Then I applied PCA to reduce the data dimensions, used K-means to cluster the cryptocurrencies, and then built some visualizations to view the results

After cleaning the dataframe to only look at tradable cryptocurrencies, I ended up with 532 tradable coins

![image](https://user-images.githubusercontent.com/114685724/222985236-4c193123-cbb1-496c-abca-5bcb70c8c607.png)

I then used PCA to reduce the data dimensions to three and applied the original index

![image](https://user-images.githubusercontent.com/114685724/222985257-2760db5d-1934-4bb0-9cb8-e834676f8d2a.png)

I then used the elbow method to determine the inertia and find the best value of k for my K-means analysis

![image](https://user-images.githubusercontent.com/114685724/222985276-018a9312-32fd-47ce-ab41-ad21ad8dba47.png)

Then, I brought in the PCA data and the Class back into the original dataset 

![image](https://user-images.githubusercontent.com/114685724/222985310-74231839-2ad0-4f3c-8679-2397ffac9cad.png)

Finally, I built visualizations!

This was a 3-d model to show the clustering and I added the algorithm and the coinName upon hovering

![image](https://user-images.githubusercontent.com/114685724/222985399-13c99d33-a3a4-4d5d-9654-4f057db9d9aa.png)

Lastly, I built a scatter plot to also show the clustering and the few outliers


## Summary

Overall, this was a super interesting analysis and it definitely shows there are a few outliers in the cryptocurrency industry: BitTorrent and TurtleCoin both had some oddities with their number of coins mined and their total supply. That deserves more research and may be why the clustering is a little odd. 

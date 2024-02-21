
## **Simple and advanced imputation; drop, mode, median, KNN, MICE**

Dealing with missing data is a prevalent and inherent challenge in data collection, particularly when dealing with extensive datasets. Numerous factors contribute to missing data, including participants providing incomplete information, non-responses from individuals who decide not to share data, poorly designed survey instruments, or the necessity to exclude data due to confidentiality concerns.

**You can read the medium article from** [Dealing with Missing Data from Zero to Advanced](https://medium.com/@hhuseyincosgun/dealing-with-missing-data-from-zero-to-advanced-4fb734ee5998)

![image](https://github.com/hhuseyincosgun/Missing-Data-Imputation-Visualization/assets/21257660/567b8ece-a135-411a-b425-efacf72afe52)


Types of Missing Data When assessing the potential impact of missing data on registry findings, it is important to consider the underlying reasons for missing data. Missing data is grouped into three categories: Missing completely at random (MCAR) Missing at random (MAR) Not missing at random (NMAR)


# Conclusion

In this article, we analyze the results by applying different methods on how to deal with missing data. In the first stage, we identified missing data and analyzed the density in the data set visually and proportionally. We continued by coding how to deal with the detected missing data.

![image](https://github.com/hhuseyincosgun/Missing-Data-Imputation-Visualization/assets/21257660/daeb3ca7-7ade-4de1-9534-2e89c95e9ab6)


-   **Removing missing data from the dataset seems to have increased the impact of outliers on std.**
-   **In mean and median imputation methods, it increases the weight at a single point. This is why std is being suppressed and causing the range to get shorter.**
-   **Knn and mice solve the problem of missing values without disturbing the normal distribution. In addition, mice seem less** **affected** **by outliers.**

First, we analyzed the results using dropping and simple imputation methods.  Mean and median imputation for a variable with a high proportion of missing data gives biased results.  Or it distorts the correlation with other variables. But we chose to go a little deeper and collaborate with other variables in the dataset. In this way, we realized that instead of considering variables separately from the dataset, it is more accurate to solve this problem by considering all variables together.

Among the advanced imputation methods, we used KNN and MICE to fill in the missing data. The result gave a fairly accurate distribution compared to simple techniques.


**_You can find the source code and_** [**_notebook here_**](https://www.kaggle.com/code/huseyincosgun/missing-data-imputation-visualization?scriptVersionId=140790877)**_._**

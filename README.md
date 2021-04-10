# Assignment: Design and Application of a Machine <br> Learning System for a Practical Problem :<br> 

>Determine customers who are likely to obtain a discounted insurance premium for the next travel and estimate its value

View Classification Solution - [Press here](https://nbviewer.jupyter.org/github/BlinkovYevhenGit/TravelInsuranceCompany/blob/main/Machine%20Learning/Completed/CE802_P2_Notebook.ipynb)

## Results of Classification

Table 1 – Comparative table of results obtained from applied classification models to the test dataset.

|                      |                      |                      **Predicted values**            |                                 |                        | 
| -------------------- | -------------------- | -----------------------------------------------------| ------------------------------  |------------------------|
| Predicted #          | K-nearest neighbours | Support vector machine with a linear function kernel | Support vector machine with rbf |  Decision trees        |
| 0                    | False                | True                                                 | False                           | False                  |
| 1                    | True                 | False                                                | True                            | True                   |
| 2                    | True                 | True                                                 | True                            | True                   |
| 3                    | False                | False                                                | False                           | False                  |
| 4                    | False                | False                                                | False                           | False                  |
| 5                    | False                | False                                                | False                           | False                  |
| 6                    | False                | False                                                | False                           | False                  |
| 7                    | True                 | True                                                 | True                            | True                   |
| 8                    | True                 | True                                                 | True                            | False                  |
| 9                    | True                 | True                                                 | True                            | True                   |
| 10                   | True                 | True                                                 | True                            | True                   |
| 11                   | True                 | True                                                 | True                            | True                   |
| 12                   | False                | False                                                | False                           | False                  |

> While considering results from the sample above we can notice one interesting detail regarding the content of table 1. In essence, the table contains two clusters of identical results from each of the methods. <br><br> Thus, this feature indicates the consistency between the forecast results of the same data and that those classifiers have very good performance. Besides that, it became clear that those classifiers can determine whether a customer is likely to get insured for the next time or not.

### Summary
> According to obtained results from the conducted investigation, we should state that we have managed to determine whether a certain customer shall obtain a discounted premium and get insured for the next time or not by applying the ML techniques.<br><br>
The list of implemented techniques includes a decision tree classifier, a support vector machine with a radial basis function kernel, a support vector machine with a linear function kernel, and a k-nearest neighbours’ classifier. Thus, by applying unique features of each method to solve the given task, all of these classifiers have provided rather fine performance both on train and test datasets. <br><br>
By the way, we can determine the strengths and weaknesses of applied methods by considering the obtained results. <br><br>
For example, the main strength of the decision tree is its powerful ability to find hidden rules from the given data and represent them as a tree. It allows anyone to better understand what are the logical connections between different variables. On the other hand, in our case, the obtained tree was too large, so it turned out hard to perceive anything. Besides that, this method is not powerful enough to achieve high accuracy on rather large volumes of real data. In addition, it has too many parameters to adjust, so it could be a hard task to find the optimal ones to reach a decent level of precision.<br><br>
In contrast, both SVM implementations have provided a decent performance on such large datasets, but the best one had a radial basis kernel which allowed it to achieve 90% of accuracy on the test data. Therefore, the main strength is their excellent performance and applicability to a vast amount of information. However, the weakness of SVM is its sensibility to a scale of data. This fact indicates that a researcher has to investigate how to standardise his raw data in order to obtain a precise model. <br><br>
The last model – k-nearest neighbours has got a similar accuracy to the decision tree one. In essence, it also has the same flaw as the decision tree method – sensibility to a volume of data, so it does not perform enough well on large datasets.<br><br>
On the other hand, it does not have many parameters to adjust. So, due to the basic idea embedded in its algorithm, it has proven its applicability to the given datasets and demonstrated a decent performance indeed.<br>

>All in all, in the result of the conducted investigation on the ML methods application to classify customers, it is stated that the given task can be solved using such classifiers as decision trees, support vector machine with a radial basis function kernel, a support vector machine with a linear function kernel and a k-nearest neighbours. Thus, in essence, a travel insurance company can apply the aforementioned techniques to get to know whether they should suggest a discounted premium further or not.

View Regression Solution - [Press here](https://nbviewer.jupyter.org/github/BlinkovYevhenGit/TravelInsuranceCompany/blob/main/Machine%20Learning/Completed/CE802_P3_Notebook.ipynb)

## Results of Regression

The difference between the accuracies of each method is demonstrated  in table 2 below. 

Table 2 – The table of comparison between actual values and predicted ones.

|        |         |                      **Predicted values**        |                  ||
|--------|---------|------------------------| ------------------------| ------------------|
| Record | Actual  | Multi-layer perceptron | Support vector machine  | Linear regression |
| 0      | 475.90  | 508.539091             | 588.486319              | 726.400002        |
| 1      | 171.50  | 158.726110             | 183.146305              | 385.820427        |
| 2      | 728.66  | 784.578626             | 913.438289              | 956.316462        |
| 3      | 0.00    | 1.177026               | -43.762342              | -344.788691       |
| 4      | 580.16  | 589.585834             | 776.467087              | 906.901620        |
| 5      | 0.00    | -2.733381              | 253.393827              | 516.467786        |
| 6      | 0.00    | -1.826787              | -33.665007              | -425.026423       |
| 7      | 2031.42 | 1960.445351            | 1764.234917             | 1761.464708       |
| 8      | 0.00    | -18.061600             | -107.127773             | -162.947552       |
| 9      | 0.00    | 0.184409               | 533.353645              | 704.834123        |
| 10     | 2908.23 | 2855.745356            | 3967.994901             | 2647.761125       |

>While comparing the actual values and predicted ones, it can be noticed that the Multi-layer perceptron model has almost identical results, which indicates its reliability and indeed excellent performance. <br><br>
In contrast to it, the Linear regression model has shown the worst prediction results that are rather distant from the real values.
It is worth mentioning a fact that SVM also finely managed with the task, because in most cases its forecasted values are rather similar to the actual ones, despite having sometimes a large bias.<br><br>

The prediction results of the final test dataset are demonstrated in the table 3 below.

Table 3 – The table of comparison between predicted values of each model

| **Predicted #** | **Multi-layer perceptron** | **Support Vector Machine** | **Linear regression** |
|:---------------:|:--------------------------:|:--------------------------:|:---------------------:|
| 0               | 502\.829691                | 537\.405356                | 739\.920670           |
| 1               | \-4\.395854                | \-99\.969252               | 275\.760310           |
| 2               | 3698\.208751               | 3248\.694602               | 2653\.437827          |
| 3               | 2470\.120800               | 2138\.339931               | 1765\.704389          |
| 4               | 2\.854894                  | \-569\.030387              | 151\.045057           |
| 5               | 2088\.009765               | 2252\.262093               | 2100\.274914          |
| 6               | 226\.007456                | 669\.279691                | 744\.634067           |
| 7               | 513\.348399                | 906\.738057                | 842\.083932           |
| 8               | \-1\.597038                | \-186\.832498              | \-107\.316205         |
| 9               | 2218\.319345               | 1998\.867712               | 1658\.471504          |
| 10              | 777\.930841                | 720\.911585                | 890\.819016           |

>From the predicted values of the best method (Multi-layer perceptron), the assumption can be made about what the real values are. For example, results -4.395854, 2.854894, and -1.597038 for the customers 1, 4, 8, accordingly, indicate that these customers shall not obtain a discounted premium for the next time.  In turn, both the other methods also provide relatively small values for these customers which implies that those people are unlikely to get insured further. 

### Summary

>According to obtained results from the conducted investigation, we should state that we have managed to predict discounted premium values for each customer and, in particular, determine whether a customer shall get insured or not simply by considering the magnitude of an outcome. <br><br>
The list of implemented techniques includes linear regression, a support vector machine with a radial basis function kernel, and a multi-layer perceptron. Thus, by applying unique features of each method to solve the given task, all of these classifiers have provided rather fine performance both on train and test datasets. <br><br>
By the way, we can determine the strengths and weaknesses of applied methods by considering the outcomes <br><br>
For example, the main strength of linear regression is a rather simple approach that allows it to get adjusted to data even with many variables. On the other hand, this technique can only work properly if the relationship between dependent and independent variables is linear. Otherwise, an application of a linear regression would not have any sense.  <br><br>
Certainly, we did not have a perfect linear relationship between the mentioned types of variables in the considered datasets. However, nevertheless, we have managed to achieve a decent precision for the linear regression model even on such large amounts of data. <br><br>
Thus, at least on average we may know for sure which customer shall obtain a discounted premium or not. Although, the actual value of a possible discounted premium is rather hard to imagine.<br><br>
In contrast, an SVM implementation has provided much better performance. Thus, an application of a radial-basis kernel to the SVM model allowed it to achieve 91.2% of accuracy on the test data. Therefore, the main strength of SVM is its excellent performance and applicability to a vast amount of information. However, the weakness of SVM is its sensibility to a scale of data. This fact indicates that a researcher has to investigate how to standardise his raw data in order to obtain a precise model. <br><br>
According to the obtained results, the SVM model, undoubtedly performs excellently, however, in some cases the outcomes have a considerable bias. Nevertheless, this model still can be used to do its job and demonstrate high accuracy.<br><br>
The last model – multi-layer perceptron has demonstrated an amazing performance on training data and prepared validation data. In essence, it managed to achieve 99.9% of accuracy and a tiny mean squared error. Considering the obtained values from the test dataset, it is expected greatly to prove its extremely high precision. <br><br>
Thus, it would be obvious to an insurance manager to determine possibly not-insured customers, because most of the obtained values are grouped around 0. <br><br>
Concerning the other values, still in some rare cases, this model has a small bias, but perhaps in a real-life, it would not be a rather big difference. <br><br>
On other hand, this model has many parameters to adjust. Therefore, it would take more time to train on a larger dataset with billions of records. Also, almost always this technique requires data scaling to work properly. <br><br>
However, the travel insurance company could take advantage of this model to precisely predict the values of discounted premiums for their customer.<br>

>All in all, in the result, of the conducted investigation on the ML methods applied to determine a value of a discounted premium, it should be claimed that the given task can be solved using such classifiers as linear regression, a support vector machine with a radial basis function kernel and a multi-layer perceptron. Thus, in essence, a travel insurance company may apply the aforementioned techniques to their needs.



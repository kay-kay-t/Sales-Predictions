In this project I'm analizing dataset and trying to make sales prediction for food items sold at various stores. The goal of this is to help the retailer understand the properties of products and outlets that play crucial roles in increasing sales.

My Project contains data cleaning and analizing, visualizations of different aspects of data and using machine learning models to see which one is doing better predictions. 
Data Dictionary for this dataset:

![image](https://user-images.githubusercontent.com/66798944/136724798-a5d3cfdb-b86e-44a4-9832-be368da562a6.png)
	
 Visualizations below show how different features of data impact sales.

1. General correlation in data, that shows what features have the most impact on sales.
![image](https://user-images.githubusercontent.com/66798944/136725365-b9fbd7d1-bf30-4930-b1e9-795dd5e46fc3.png)

 Visualization above shows that Item Max Retail Prise has high impact on Outlet Sales

2. Let's see Max Retail Prise distribution to have better understanding of it
![image](https://user-images.githubusercontent.com/66798944/136725494-81020329-676c-408d-94bd-b000431b99ad.png)

 This histogram shows that the most amount of items priced at range of 100 to 125. The least amount is in price range between 200 and 225

3. Visualization below shows which item types are selling the most and the least. That can give an idea, which items the store should try to sell more.
![image](https://user-images.githubusercontent.com/66798944/136725958-b4144a02-05bf-4fff-991c-5114f4a4d986.png)

 Per visualization above we see, that the most selling items are Starchy Foods, Seafood and Fruits and vegetables. Stores could consider decreasing prices on Baking Goods, Soft Drinks and Health&Hygen or run some promotions to increase those items sales.

4. Next visualization shows how outlet size affect sales.
![image](https://user-images.githubusercontent.com/66798944/136726422-6be8583c-fab7-4dc4-89b1-c41015ec9cdd.png)

 Since sales are the highest at medium sizze stores, if retailer considering on openning new stores, they should take this into consederation in order to improve sales.

In next part of project I am using different prediction models, such as Linear regression, Decision Tree model, Bagged Tree model and Random Forest model. 
After applieng all four of them to this dataset, I am comparing the results:

1. Lenear Regression Model:
0.5660618087246838
0.5606446946459837
2. Decision Tree Model:
1.0
0.15930919901843388
3. Bagged Tree Model:
0.9182102766404884
0.5153952406542452
4. Random Forest Model with max_depth of 5:
0.619882193339827
0.6024842557552188

Those numbers indicate, that Random Forest Model with max_depth of 5 can give the most accurate predictions. 

Also, I'm comparing RMSE:

1. Linear Regression Model:
Training RMSE: 1140.2861766872174
Testing RMSE: 1094.1780540846619
2. Decision Tree Model:
Training RMSE: 0.0
Testing RMSE: 1522.9730220775825
3. Bagged Tree Model:
Training RMSE: 491.9888854109978
Testing RMSE: 1156.2930098370166
4. Random Forest Model with max_depth of 5:
Training RMSE: 431.589518411024
Testing RMSE: 1121.1120993931045

Random Forest model has second smallest error and did the best on predictions. So I would recommend using Random Forest model with max depth of 5 for this dataset.

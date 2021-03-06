# Linear Regression : Overview
In this project i used data from [E-Commerce Data](https://github.com/denidya/linear-regression/blob/main/Ecommerce%20Customers) and doing little exploration data analysis to see correlation between feature.

## Codes & Resources Used
- Editor Used : VS Code
- Python version : 3.8.8
- Package used : numpy, pandas, matplotlib, seaborn
- sklearn

## About Dataset
This data have info such as Email, Address and color avatar. Then it also have numerical value columns:
- Avg. Session Length: Average session of in-store style advice sessions.
- Time on App: Average time spent on App in minutes
- Time on Website: Average time spent on Website in minutes
- Length of Membership: How many years the customer has been a member.

## Some Correlation chart
- Time on Website vs Yearly Amount Spent <br />
  ![time on website vs yearly amount spent](https://user-images.githubusercontent.com/41662335/145139027-1d1a0cf6-635f-41e7-afdc-e1adbec29daa.png)
- Time on Apps vs Yearly Amount Spent <br />
  ![time on apps vs yearly amount spent](https://user-images.githubusercontent.com/41662335/145139164-9b533078-21a8-4745-b3b6-9a8ab86af99a.png)
- Length of Membership vs Yearly Amount Spent <br />
  ![length of membership vs yearly amount spent](https://user-images.githubusercontent.com/41662335/145139213-88b3054d-5a7f-4760-a7e2-7088ccbf0d77.png)

## Comparation Test Data & Prediction 
![scatterplot real test vs prediction](https://user-images.githubusercontent.com/41662335/145139557-29563df0-992f-44a9-9ec2-33e3745535b7.png)

## Evaluating Model
- Calculate MAE (Mean Absolute Error), MSE (Mean Squared Error), RMSE (Root Mean Squared Error)
  | Metrics       | Residual      | 
  | ------------- | -------------:| 
  | MAE           | 7.2281        | 
  | MSE           | 79.8130       | 
  | RMSE          | 8.9338        | 

- Check Residual/Data Distributed <br />
  ![residual](https://user-images.githubusercontent.com/41662335/145140823-7855750f-66e1-433e-82ff-cd78a5a956ff.png)
 
## Conclusion
- Check Coefficient
  | Feature               | Metrics    | 
  | --------------------- | -----------| 
  | avg_session_length    | 25.981550  | 
  | time_on_app           | 38.590159  | 
  | time_on_website       | 0.190405   |
  | length_of_membership  | 61.279097  |
  
- Interpreting Coefficient <br />
  Increasing 1 unit in **avg_session_length** means increasing **25.98 dollars spent.** <br />
  Increasing 1 unit in **time_on_app** means increasing **38.59 dollar spent.** <br />
  Increasing 1 unit in **time_on_website** means increasing **0.90 dollars spent.** <br />
  Increasing 1 unit in **length_of_membership** means increasing **61.27 dollars spent.** <br />


### Mini Project for Team of 
#### Pankaj Suresh Kumar, Kalpesh Mulye, Raja Mohanty




### EDA

1. Target(Y) split across Yes/No

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/MicrosoftTeams-image1.png)

2. Missing Values

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA2.png)

3. Coorelation Matrix 

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA3.png)

4. Summary/Frequency Distribution of predictors :

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA4.png)



![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA5.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA6.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA7.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA8.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA9.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA10.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA11.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA12.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA13.png)

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/EDA14.png)



### K - means

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/Mod_eval01.png)
![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/Mod_eval02.png)
###



##Model Evaluation 

### Logisitic Regression

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/Model_Eval1.png)

### Decision Trees

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/Model_Eval2.png)

### Random Forest

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/Model_Eval3.png)

###Gradient Boosted Trees

![alt text](https://github.com/kalpesh22-21/miniproject/blob/main/images/Model_Eval4.png)


From all the 4 above models we see that the Gradient boosting model had the highest accuracy of 91.11% and precison of  50% in predicting "YES" class i.e. those who are likely to do a deposit.


# Deploy
 Flask deployment file [deploy](https://github.com/kalpesh22-21/miniproject/blob/main/flaskdeploy.py) is added.
 There are two app routes in the file namely
 1. "/" route - returns index.html
 2. "/predict" route - accepts list of inputs as shown below
 
 ```python
 input_string - "51,technician,single,professional.course,no,no,no,cellular,aug,wed,
                 1740,1,999,0,nonexistent,1.4,93.444,-36.1,4.964,5228.1,no"
 columns - ['age', 'job', 'marital', 'education', 'default', 'housing', 'loan',
            'contact', 'month', 'day_of_week', 'duration', 'campaign', 'pdays',
            'previous', 'poutcome', 'emp_var_rate', 'cons_price_idx',
            'cons_conf_idx', 'euribor3m', 'nr_employed', 'y']
 ```
 Finally Returns if person is likely to do deposit as "Yes" or "No"
 

# Bank_fraud_classification

## approach :
- Data Discovery 
- preprocess train data
- preprocess test data
- build models 
- predict for test data

### Data Discovery 

- Checked for missing Data for categorical and numeric variables 
- Analysed distributions and behaviour of data 
- Parameters with more than 50% data missing , are ommmited , it can be handlled , but needs more time 
- Parameters with less missing values are handlled by various techniques like random imputation, replace with mean 
- data replacement strtegies are decided as per data behaviour (details are in the Data Descovery Notebook) 
- Please see Data Discovery Notebook for detailed analysis 

### Data preprocessing 

- categorical feature are encode with various techniques eg. lable encoding, count frequency and target encoding 
- Some of the text columns are ommited , idea was to train separate sentiment analysis model and then code it with sentiemnt (lack of time) 
- For details please see Preprocess Train Data notebook 
- same steps are done to process test data 
- For encoding of Test data , model was fitted on train data and done transformation for test data 
- Please watch Preprocess Test data Notebook 
- Feature selection is done with lasso regression 

### model training 

- Data is scaled (though it wont effect much on tree based models)
- Done data split for train data
- Trained Random forest, Xg boost and Logistic Regression models 
- Check for classification report for test data 
- Done prediction on test data 

### Future scope 

- need to do Hyper parameter tuning using Grid CV 
- need to do K fold cross validation 

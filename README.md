
# SALES PREDICTIONS 

**Author**: Milene Carmes Vallejo 

### Business problem:

This project is a sales prediction for food item sold at various stores. The price is in Indian Rupee, the rate is: 1 indian ruppe is about 0.012 USD. 


### Data:
Original data source is from https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

Here is the Data Dictionary for this dataset

![sales_predictions](Picture1.png)



## Methods


Predictions part
- Data preparation: check duplicates, fix inconsistencies in Item_Fat_Content column, check dtype of all columns. 
- Train/Test split: "Item_Outlet_Sales" column as target.
- Make selector columns because there are numbers and objects columns in this dataset.
- Ckeck missing values: There are missing values in numeric column Item_Weight that is float number and there are missing values in categorical column Outlet_Size. I used SimpleImputer the ‘mean’ strategy for numeric columns (that is a float number) and SimpleImputer the ‘most_frequent’ strategy for categorical columns.
- I used OHE for categorical columns and scaler for numeric columns since in machine learning the dataset needs to be all numeric and in the same scale. 
- I made a numeric_pipe and categorical_pipe with make_pipeline. 
- I created tuples for numeric and categorical where the first element is the transformer and second element is a ColumnSelector oject
- I used make_column_transform to put all together (numeric and categorical tuples)
- I used 3 Models :  linear regression model, Decision Tree Regressor and Randon Forest 
- Evaluated the performance of 3 models based on r^2 and used regression metrics (MAE, MSE, RMSE).
- Compared 3 different models. 



## Results

### Here are examples of how to embed images from your sub-folder


#### Visual 1 Title
![sample image](project1_sample_image.png)

> Sentence about visualization.
#### Visual 2 Title

## Recommendations:

More of your own text here


## Limitations & Next Steps

More of your own text here


### For further information

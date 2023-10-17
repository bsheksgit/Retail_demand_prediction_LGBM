# Retail demand prediction using Light GBM

CSV Files:

* train.csv contains data about the date, store number, Unique product code, base price, feature, display and the number of units sold.
* Contains columns: WEEK_END_DATE	STORE_NUM	UPC	BASE_PRICE	FEATURE	DISPLAY	UNITS
* final_data.csv is the already preprocessed dataset.
* Contains the columns: 
WEEK_END_DATE	STORE_NUM	UPC	BASE_PRICE	FEATURE	DISPLAY	UNITS	MANUFACTURER_1	MANUFACTURER_2	MANUFACTURER_3	MANUFACTURER_4	MANUFACTURER_5	MANUFACTURER_6	MANUFACTURER_7	MANUFACTURER_8	MANUFACTURER_9	CATEGORY_1	CATEGORY_2	CATEGORY_3	CATEGORY_4	SUB_CATEGORY_1	SUB_CATEGORY_2	SUB_CATEGORY_3	SUB_CATEGORY_4	SUB_CATEGORY_5	SUB_CATEGORY_6	SUB_CATEGORY_7	PRODUCT_SIZE	year	month	day	day_of_year	week	quarter	U_MANUFACTURER	U_CATEGORY	U_SUB_CATEGORY	UNITS_BEFORE_52WEEK	price_difference	2_MONTH_BEFORE	1_WEEK_BEFORE	AVERAGE_UNITS_IN_2_MONTH

* product_data and store_data contain data about the various products and stores.

.ipynb file:

* LGBM regressor is trained on the train.csv dataset.
* Root mean square log error is used to evaluate the model.
* Most important features of the map are plotted in the end.
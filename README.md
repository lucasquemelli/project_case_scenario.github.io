# project_case_scenario.github.io
This is a project about investing in Residential real estate.

In this assignment, I worked at a Real Estate Investment Trust. The Trust would like to start investing in Residential real estate. I was tasked with determining the market price of a house given a set of features. I analyzed and predicted housing prices using attributes or features such as square footage, number of bedrooms, number of floors, and so on.

# House Sales in King County

This dataset contains house sale prices for King County, which includes Seattle. It includes homes sold between May 2014 and May 2015.

![image](https://user-images.githubusercontent.com/81119854/128383355-ab16bde1-fd1c-4276-b205-66975ce92f45.png)

# Libraries used in this project

![image](https://user-images.githubusercontent.com/81119854/128383570-5ffeade2-282d-4ae6-9050-4db9f8968736.png)

# Importing Data Sets

Load the csv:

![image](https://user-images.githubusercontent.com/81119854/128383708-25ef7cbc-6b4f-4e14-96e6-95187548f75c.png)

We use the method head to display the first 5 columns of the dataframe.

![image](https://user-images.githubusercontent.com/81119854/128383803-b4ad51a9-c372-4c6e-aef7-71370502dd9a.png)

![image](https://user-images.githubusercontent.com/81119854/128383872-9cd69771-0d84-4907-93e7-85850eb6be6e.png)

![image](https://user-images.githubusercontent.com/81119854/128383915-ed3ffec2-3bd3-49d3-a1ae-028cc73e24b4.png)

We use the method describe to obtain a statistical summary of the dataframe.

![image](https://user-images.githubusercontent.com/81119854/128384000-901aa25a-40e0-4776-b8a1-3fc5133b68e6.png)

# Data Wrangling

![image](https://user-images.githubusercontent.com/81119854/128384291-a1026e16-fe1b-491d-9bb0-17a97203fb86.png)

![image](https://user-images.githubusercontent.com/81119854/128384566-32e64f66-1f72-4142-96be-c4fc31538b71.png)

We can see we have missing values for the columns  bedrooms and  bathrooms 

![image](https://user-images.githubusercontent.com/81119854/128384660-43e024d7-3527-4e78-8fc8-3702bca89ac7.png)

We can replace the missing values of the column 'bedrooms' with the mean of the column 'bedrooms'  using the method replace(). We set the inplace parameter to True

![image](https://user-images.githubusercontent.com/81119854/128384784-0b438f1e-4541-44e9-8090-7601b94117ff.png)

We also replace the missing values of the column 'bathrooms' with the mean of the column 'bathrooms'  using the method replace(). We set the  inplace  parameter top  True

![image](https://user-images.githubusercontent.com/81119854/128384973-59e80de2-ccce-43ac-b5f9-1ff50a7a2915.png)

All missing values from the columns bedrooms and bathrooms were droped:

![image](https://user-images.githubusercontent.com/81119854/128385119-a3caa2c1-7a4b-4b76-a491-616ad4aa5e44.png)

# Exploratory Data Analysis

![image](https://user-images.githubusercontent.com/81119854/128385325-d7f2bc03-8c31-49ab-957e-62304efd95be.png)

![image](https://user-images.githubusercontent.com/81119854/128385374-6696348b-7490-4665-89e7-45f6fdd45fab.png)

![image](https://user-images.githubusercontent.com/81119854/128385460-80757996-2666-4a9e-9502-98ad627678ad.png)

![image](https://user-images.githubusercontent.com/81119854/128385518-a3bbbf56-4e47-4de4-89c4-ed723caa9685.png)

The houses without a waterfront view has much more price outliers.

![image](https://user-images.githubusercontent.com/81119854/128385823-56bbbb75-e6d8-4493-99a1-5004aa1be9b3.png)

![image](https://user-images.githubusercontent.com/81119854/128385884-393bfb9f-df30-4adb-bc44-4284ea81ead7.png)

Square footage from house apartment from basement (sqft_above) is positively correlated with price. 

We can use the Pandas method corr() to find the feature other than price that is most correlated with price.

![image](https://user-images.githubusercontent.com/81119854/128386452-ff3aac39-acb2-446b-86e2-c4208e58a126.png)

The living room area (sqft_living) is the feature that is most correlated with price. It suggests that better investments is this area probably could improve the value of a house as well as it would improve its sale profit.

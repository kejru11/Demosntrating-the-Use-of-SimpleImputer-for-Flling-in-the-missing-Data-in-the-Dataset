# Demosntrating-the-Use-of-SimpleImputer-for-Flling-in-the-missing-Data-in-the-Dataset

SimpleImputer is a class in the Scikit Learn library that is used for filling in the missing data that we usually encounter when dealing with real life datasets. 

In the given program, I have taken the help of a car-dataset that contains the details of a car dealership that deals in used cars. There are over 1000 rows or car entires, and there are plenty of data missing. 

In order to efficiently train our machine learning model, it is required that we first fill the missing data, and then proceed with training our machine learning models. 

In the given repository, you will find three files:

        a. "car-sales-extended-missing-data": This CSV file contains the car details, and there are over a 1000 different entries. The file has missing entires that we             are trying to eliminate. 

        b. "filling in the missing data using the Simple Imputer Function": This python file consists of the code that I have written to fill in the missing data. I               have created the use classes for the SimpleImputer, and then I have implemented the changes in the dataset using the ColumnTransformer class. 

        c. "updated_dataset": The Updated Dataset is the file I have extracted after implementing the changes using the SimpleImputer function. There are five                     different rows in the dataset:

            1. Make: Make is the manufacturers of the car. Because it takes a string value, I have filled the missing entries with the keyword "Missing"
            2. Colour: The Colour column contains the colour of the car. Because it takes a string value, I have filled the missing entries with the keyword "Missing"
            3. Doors: The Doors column contains the number of the doors in the car. After running the sum function on the column, I found that there are over 850+                    entries with 4 door cars. This is the reason why I have filled in the missing data with 4. 
            4. Odometer (KM): Odometer KM is a numeric value and it contains the numer of KM for which the car has been driven. I have replaced the missing columns                    with the mean value of the coloumn of KM driven. 
            5. Price: Price is a numeric value and it contains the price for which the car is being sold. I have replaced the missing columns with the mean value of                  the coloumn of Price given. 



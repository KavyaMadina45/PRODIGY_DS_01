## Population Data Visualization Project
This project involves loading population data from an Excel file and performing various data visualization tasks using Python libraries such as pandas, numpy, and matplotlib.
The visualizations include bar charts and histograms to represent the distribution of age and gender in the dataset.

**Project Description**
The project demonstrates how to:

1) Load data from an Excel file using pandas.
2) Select and print specific columns from the data.
3) Configure pandas display options to show all rows and columns.
4) Create bar charts and histograms using matplotlib to visualize the distribution of age and gender.
   
**Installation Instructions**
To run this project, you need to have Python installed along with the following libraries:
 pandas
 numpy
 matplotlib
**Usage**
Place your Excel file containing population data (e.g., Population..xlsx) in an accessible directory.
Update the file path in the code to match the location of your Excel file.
Run the script to see the visualizations.

**Example code**
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

**Load data from Excel file**
x = '/home/kavya/Documents/Population..xlsx'
df = pd.read_excel(x)

**Display first 10 rows of specific columns**
particular_column = df[['Age', 'Gender']]
print(particular_column.head(10))

 **Configure pandas to display all rows and columns**
pd.set_option('display.max_rows', None)
pd.set_option('display.max_columns', None)

## Bar chart visualization
age_data = df['Age']
gender_data = df['Gender']
plt.xlabel('Gender')
plt.ylabel('Age')
plt.title('Distribution of Age and Gender using Data Visualization like bar charts')
plt.bar(gender_data, age_data, width=0.7, color='yellow')
plt.show()

# Histogram visualization
plt.xlabel('Age')
plt.title('Distribution of Age and Gender using Data Visualization like histogram')
plt.hist(age_data, bins=2, color='pink')
plt.show()

# Alternative histogram visualization
plt.xlabel('Age')
plt.title('Distribution of Age and Gender using Data Visualization like histogram')
plt.hist(gender_data, bins=2, color='green')
plt.show()

**Features**
1) Data Loading: Efficiently loads population data from an Excel file.
2) Data Selection: Prints specific columns (Age and Gender) for inspection.
3) Display Configuration: Adjusts pandas settings to show all data without truncation.
4) Bar Chart Visualization: Creates bar charts to visualize the relationship between age and gender.
5) Histogram Visualization: Creates histograms to visualize the distribution of age and gender.
   
**Contributing**
If you want to contribute to this project, please follow these steps:

* Fork the repository.
* Create a new branch (git checkout -b feature-branch).
* Make your changes.
* Commit your changes (git commit -m 'Add new feature').
* Push to the branch (git push origin feature-branch).
* Create a new Pull Request.
**License**
  This project is licensed under the MIT License - see the LICENSE file for details.
*Contact Information*
 For any questions or issues, please contact Kavya at madinakavya6@gmail.com 



Spyder Editor

This is a temporary script file.
"""

# Assignment-1
#This is the Assingment 1
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

# Reading the data from the excel file
df = pd.read_excel('C:\Users\DELL\Downloads\Data_tables_for_Malpractice_for_GCSE__AS_and_A_level_summer_2018_exam_series.xlsx')

# Creating a bar graph using the data
plt.bar(df['year'], df['entries'])

# Setting the title and labels for the axes
plt.title('Number Of Candidates 2011 - 2015')
plt.xlabel('Year')
plt.ylabel('Candidates')

# Displaying the bar graph
plt.show()



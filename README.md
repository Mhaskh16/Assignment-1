# Assignment-1
#This is the Assingment 1
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

# Reading the data from the excel file
df = pd.read_excel(r'C:\Users\DELL\Downloads\Data_tables_for_Malpractice_for_GCSE__AS_and_A_level_summer_2018_exam_series.xlsx')

# Creating a bar graph using the data
plt.bar(df['year'], df['entries'])

# Setting the title and labels for the axes
plt.title('Number Of Candidates 2011 - 2015')
plt.xlabel('Year')
plt.ylabel('Candidates')

# Displaying the bar graph
plt.show()

# creating Pie Chart

years = df["year"].tolist()
candidates = df["entries"].tolist()


plt.pie(candidates, labels=years, autopct="%1.1f%%")
plt.axis("equal")

# displaying Pie Chart
plt.show()

# creating Scatter plot
def create_scatter_plot_top_10(df, x_column, y_column, title, xlabel, ylabel):
    plt.figure(figsize=(10, 6))
    plt.scatter(df[years], df[entries], alpha=0.5)
    for i, row in df.years():
        plt.text(row[x_column], row[y_column], row['iso3c'], fontsize=9)
    
    plt.title(title)
    plt.xlabel(xlabel)
    plt.ylabel(ylabel)
    plt.grid(True)
    
#Displaying Scatter Plot
    plt.show()



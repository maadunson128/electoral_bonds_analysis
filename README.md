
# Electoral Bonds Analysis

I am going to do a Analysis on the data related to Electoral Bonds released by SBI on the advise of Supreme Court on March 2024.

The entire flow will added below as my progress continues.


## Overall Flow

### 1. Knowledge about the Electoral bonds
Listened to some podcasts related to Electoral bonds and some articles on this topic.


### 2. Downloading data
Downloaded the 2 PDF's released by SBI from the following link:
###
    https://www.eci.gov.in/disclosure-of-electoral-bonds

It will be located in the data folder in this repo.


### 3. Manual Overview
Overviewed the data in each PDF's and understood the meaning of the columns.

### 4. Converting the PDF's into suitable data format
I thought of two data formats(csv, xlsx) to convert the data in PDF.
I converted the PDF's to csv using online websites but the output format wasn't not satisfied.
I tried to something with the csv file where its format was not satisfied. It made me took many hours ended to give up.
Then searched for any PDF related libraries in python to modify the PDF's to csv. I came up with library 'tabulu-py' which can be useful with tabular PDF.
I will try the library and update the flow.

### 5. PDF's into csv
After some basic knowledge of some useful functions such as read_pdf() in tabula and concat(), to_csv() in pandas, the two PDF's is converted into csv files.
The csv files were checked with the PDF manually by cross checking the number of rows in each PDF along with the converted csv's.

### 6. Using Google Collab
I can't use jupter notebook for my further analysis since my laptop doesn't have high specifications to process the data. So, I opt for google collab.
I uploaded the csv files into google drive and mounted the google drive in my collab notebook.
From now on, the EDA and other analysis will be carried on the google collab.

### 7. Modifications in dataframe
Merged the two dataframes on column 'UniqueID' which was created by merging the columns 'Prefix' and 'BondNumber' on two dataframes.
Found an interesting thing related to number of bonds purchased and encashed.(Included in the notebook).

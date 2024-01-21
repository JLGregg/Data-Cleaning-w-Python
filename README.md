# Cleaning Data using Pandas in Jupyter Notebook

### Project Description
In this project, I am taking a dataset that I downloaded from Kaggle and cleaning the data using Pandas to make the data better for analysis.

### Data Source
I will be using the Coffee Bean Sales Raw Dataset. This is found on Kaggle at the following link: https://www.kaggle.com/datasets/saadharoon27/coffee-bean-sales-raw-dataset <br>
The file had a few empty headers which I removed.

### Tools
- Jupyter Notebook
- Python
- Pandas

# Cleaning the Data
First I imported the data and used a try-catch block to read the Excel file. I brought in all three sheets of the Excel file to condense them down into one data set with the needed data to answer the following questions: 
- How do my coffee sales change over time for each type?
- Where do I sell the most coffee?
- Who are my top 5 customers?
- Which roast type sells the most?

I do not answer these questions in this project but the project I did answer these questions can be found here https://github.com/JLGregg/coffee_data_analysis <br> 
In that project I cleaned the data with Excel, used SQL queries, and visualized with Tableau.

![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/c1550d02-ec34-42cf-9bec-da51643228ed)<br>
This is the code I used for importing and printed out the top 5 rows of each sheet.
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/7190575d-e5ed-44ed-8d0b-7d6f27c0961e) <br>

The first thing I did after bringing in the data is merge the data from the customer and products Excel worksheets to the Orders worksheet.
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/da653684-ed93-4b2c-b902-1e0c33a97498) <br>

After merging the data, I then checked the data types <br>
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/54421c35-05b4-4470-809b-c9f7fdee53c3) <br>

Everything looked good so I then checked for null values <br>
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/5e21c549-2d7c-4f01-a0f2-2f36bd3855c4) <br>

I found that I do have null values in the email column but since that will not impact the questions I am trying to answer, I will leave them null.

I then changed the date format to be more readable.<br>
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/5789efec-d4a1-439b-96b9-7e645f478126) <br>

After changing the date I changed the coffe type column and roast type column to have the whole word instead of an abbreviation.
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/507ab859-31cd-4623-8078-a68dec4f7eba) <br>

I then rounded the unit price column to two decimal places
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/7411330c-31b3-4e66-b7f4-990602134d05) <br>

I checked the data types again and after I formatted the date, it was changed to an object. I converted the date back to datetime.
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/900c18fa-1218-49f5-aea8-2f6e95f0dfee)

![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/85e35fcd-ea2b-4b72-a465-632162ed54b9)

Here are the top 10 rows of the final product.
![image](https://github.com/JLGregg/Data-Cleaning-w-Python/assets/38503403/bfddf27c-34fd-448f-a270-d642be07c569) <br>

I believe by cleaning the data, it allows better analysis and an easier time answering the questions that need to be answered and a better way to bring in the data to start your visualization process.










# Titanic_Lab
Jupyter Notebook
README.md
Last Friday at 3:03 PM
GitHub Flavored Markdown
File
Edit
View
Language
1
# Lab: Titanic EDA
2
​
3
This week was all about Pandas and plotting. At this point you should be chomping at the bit to get your hands dirty on a real-world dataset.
4
​
5
For this lab, we're going to take a look at the Titanic manifest. We'll be exploring this data to see what we can learn regarding the survival rates of different groups of people.
6
​
7
## Prework
8
Fork and clone this repo. At the end of this lab, you'll submit a pull request using the `Titanic.ipynb` notebook to answer the questions below.
9
​
10
## Step 1: Reading the data
11
​
12
1. Go to [https://www.kaggle.com/c/titanic/data](https://www.kaggle.com/c/titanic/data)
13
2. If you scroll down the page a bit, you'll see a data dictionary explaining each of the columns. Take a minute to familiarize yourself with how the csv is structured.
14
4. Download the `train.csv` file into this project
15
3. Create an iPython notebook and load the csv into pandas.
16
​
17
## Step 2: Cleaning the data
18
1. Create a bar chart showing how many missing values are in each column
19
2. Which column has the most `NaN` values? How many cells in that column are empty?
20
3. Delete all rows where `Embarked` is empty
21
4. Fill all empty cabins with **¯\\_(ツ)_/¯**
22
​
23
Note: `NaN`, empty, and missing are synonymous.
24
​
25
## Step 3: Feature extraction
26
1.  There are two columns that pertain to how many family members are on the boat for a given person. Create a new column called `FamilyCount` which will be the sum of those two columns.
27
2. Reverends have a special title in their name. Create a column called `IsReverend`: 1 if they're a preacher, 0 if they're not.
28
3. In order to feed our training data into a classification algorithm, we need to convert our categories into 1's and 0's using `pd.get_dummies`
29
  - Create 3 columns: `Embarked_C`, `Embarked_Q` and `Embarked_S`. These columns will have 1's and 0's that correspond to the `C`, `Q` and `S` values in the `Embarked` column
30
  - Do the same thing for `Sex`
31
  - BONUS: Extract the title from everyone's name and create dummy columns
32
​
33
## Step 4: Exploratory analysis
34
1. What was the survival rate overall?
35
2. Which gender fared the worst? What was their survival rate?
36
3. What was the survival rate for each `Pclass`?
37
4. Did any reverends survive? How many?
38
5. What is the survival rate for cabins marked **¯\\_(ツ)_/¯**
39
6. What is the survival rate for people whose `Age` is empty?
40
7. What is the survival rate for each port of embarkation?
41
8. What is the survival rate for children (under 12) in each `Pclass`?
42
9. Did the captain of the ship survive? Is he on the list?
43
10. Of all the people that died, who had the most expensive ticket? How much did it cost?
44
11. Does having family on the boat help or hurt your chances of survival?
45
​
46
## Step 5: Plotting
47
Using Matplotlib and Seaborn, create several charts showing the survival rates of different groups of people. It's fine if a handful of charts are basic (Gender, Age, etc), but what we're really looking for is something beneath the surface.
48
​




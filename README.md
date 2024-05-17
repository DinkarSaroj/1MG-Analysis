#  1Mg Homeopathic Analysis

## Objective:
         - You are hired in a consultancy firm, one of their client want to open a homeopathic medicine store what is their total cost 
           for open their store.
         -  Create an interactive dashboard for them to analyze and select best medicine for their store. (Use benefit area as a filter)
         - Utilize a sentiment analysis library such as NLTK (Natural Language Toolkit) or TextBlob to analyze the sentiment of the 
            extracted review text.

Scrape the homeopathic medicine data from online medicine delivery platform 1mg using python library called Beautifulsoup (or similar) and collect information in the given format and make 2 tables using the data:
 
## Table 1 : medicine_name


### Attributes in table - 2:

name - Name of the medicine

size_of_the_bottle - Size of the medicine bottle or pack MRP_of_the_bottle - MRP of the bottle

price_of_the_bottle - Selling price of the bottle 1mg_url - 1mg url where the medicine sold

## Table - 2 : medicine_details
### Attributes in table - 2:

name - Name of the medicine

brand_name - Brand name

key_benefits - Key Benefits area (Hair, eye, joint, skin)

key_ingredients - Ingredient of medicine

rating - user rating of the medicine

number_of_rating - Number of people rated that product

Our goal is to clean and do a complete analysis and interpretation of the dataset. 

## Data Cleaning:
The cleaning phase is very important: without a good cleaning, our analysis could be badly influenced by outliers. So,
we decided to identify our neer during the analysis phase, to drop the useless column and clean the usefull ones.

### Identifing the needs:
To proceed to the analysis, we needed a clean dataset containing at least:
Prices, Medicine name  and Brand names.
A price/m2 column
Removing the outliers (error, incorrect or absurd).
It's good to have a lot of columns, as it can create more correlations between them. However, it's bad to have columns with errors,
incorrect, missing or absurd values. That's why we divided our cleaning in two phases:

### Cleaning the raw:
A very first clean to the raw data. We were focused on "dropping the big lies":
Dropping the duplicated rows
Dropping columns with only one unique value
Checking each columns's properties


### Refining the values

Some tweaks were made on the dataset to remove outliers and useless columns, due to their high rate of None value. This steap required deeper investigation intop the data:

## Data Analysis & Interpretation
This is where the fun start ! 🥳


To get the most out of our data, and to allow each of us to get experience manipulating Pandas and Seaborn, we decided to work separately.
Later we reviewed our work and merged the results.

Our target: The Price,  Best Brands and Review .
The price ,Review and Brand is obviously the target of this challenge, as our goal is to to create a machine learning model to predict Sentiments of Reviews.

## Challenge's answers:
- 
    - Number of medicine available of different benefit area.
   ![You can Find Number of medicine available per benifit](https://github.com/DinkarSaroj/1MG-Analysis/assets/156825223/c0388389-76da-4f00-ac90-0fc8f9dd59f5)

   
    - Price range of medicine for each benefit area.
   
    ![image](https://github.com/DinkarSaroj/1MG-Analysis/assets/156825223/6f8a172d-737c-4b33-bfa4-c4773b2bfbea)


    
    - Average price, min price , max price and number of products for each brand.
    - ![image](https://github.com/DinkarSaroj/1MG-Analysis/assets/156825223/22b32acf-010d-4ca9-9ed3-3af9837952f9)

    
    - Average number of rating for each brand in their specialization products where  the number of rating is not NULL.
    ![image](https://github.com/DinkarSaroj/1MG-Analysis/assets/156825223/91587158-a6f2-441e-9b24-20780ea3a5fd)
## Dashboard:
![1mgDashboard](https://github.com/DinkarSaroj/1MG-Analysis/assets/156825223/baf0ffb5-597c-48a6-b6e1-217fab7d0c90)

   
    
    

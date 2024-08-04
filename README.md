# Consumer's basket: aid for consumers or gift for the supermarkets? 

This is my second complete project for the LEDE Program 2024, at Columbia Journalism School.

Find the website [here](https://dafnikaravola.github.io/consumer's%20basket/)

## The goal:

Consumer's Basket was advertised as a government initiative to help combat soaring prices in basic grocery necessities. But does it truly provide relief for consumers, or is it designed to benefit supermarket chains?

**The analysis attempts to find out if the Consumer’s Basket products are indeed the cheapest available in the market.**
**And whether the largest supermarket chains utilize this measure to promote their own products and increase their turnover?** 

## The datasets:

The project is based on datasets retrieved from the Greek State's Online Market Observatory [e-katanalotis](https://e-katanalotis.gov.gr/) for the week of 26 - 30 July 2024.

E-katanalotis is a web repository of all product prices available in Greek supermarkets, delivered daily by each merchant. 

Moreover, the website offers a weekly database of all the products included in the Consumer's Basket, for all participating merchants. The dataset is renewed every Wednesday.

The datasets for all products (`prices.json`) and consumer's basket products (`basket.json`) were

## Important Findings

* Consumer's Basket includes a little less than 1 out of 10 products in the market
* The government has set a minimum of 51 distinct product categories that represent basic goods which a household needs weekly.
* Merchants include at least one product per category. Some merchants added more categories (maximum is 56).
* On average 7 out of 10 products in the basket are indeed the cheapest market option.
* Top 10 product categories for which the less expensive products cannot be found inside the basket are baby diapers, baby wipes, sanitary pads and tampons, dishwasher detergents as well as all types of coffee.
* One in two supermarkets use the basket as a chance to promote their own-manufactured products.
* Merchants who are more likely to include the cheapest categories in their basket are also more likely to promote their private labels within those categories.

## Data Analysis & Visualisation

The following tools have been used: 

**Data Analysis**

* **Json &Pandas Libraries and Jupyter Notebook:** Were used to retrieve the json file from e-katanalotis, convert the json file into a dataframe and analyse this dataframe.

**More specifically:**

To retrieve and analyse general products' data: 
- `categories_suppliers_merchats_products_29-07-2024.json` : json file from e-katanalotis
- `Products & Merchants & Categ_29-07-2024.ipynb` : Jupyter Notebook (retrieves, cleans and analyses data)
- `df_products_alldata_26-30 July 2024.csv` : the cleaned dataframe for all market products

To retrieve and analyse basket products' data: 
- `basket.json` : json file from e-katanalotis
- `Kalathi_nikokiriou_26-30 July 2024.ipynb` : Jupyter Notebook (retrieves, cleans and analyses data)
- `kalathi-nikokyriou-26-30_07_2024.csv` : the cleaned dataframe for basket products

To compare and analyse the relationship between general market products and basket products:
- `Price Comparison Analysis.ipynb` : Jupyter Notebook

Please read the Jupyter Notebooks for detailed methodology and steps explanation.

**Visualisation**
* **Flourish** : for all charts

**Website**
* [Soma's templates](https://jsoma.github.io/page-templates/https://jsoma.github.io/page-templates/)


## Skills & Approaches

**Successes**

This project was focused more on data analysis through Python and Pandas and less on exploring new visualisation methods. 
I successfully learned to retrieve a json file from the web and convert it into a dataframe. This part was particularly difficult due to the deep level of nesting in the json files. 
Moreover, this project was very useful for learning to clean a complex dataset, work with different datasets and combine them, and conduct complex levels of analysis.  

**Yet to do**

I need to set more focused questions. Sometimes I got lost in the dataset. 
I need to organise my files better. 
I need to learn how to retrieve json files weekly through github actions. 

# From Raw Records to Business Insights: A Python Analytics Project

## 📌 Project Overview
This project demonstrates how raw business data can be transformed into meaningful insights using Python.
I personally `collected 2 months` of real-world business data from a local fiber welding repair shop and built a complete analytics workflow—from data collection and cleaning to exploratory data analysis (EDA) and visualization.
The objective of this project is to show how data-driven insights can help small business owners understand their operations, identify opportunities for growth, and make informed business decisions.

## 🪟 Business Overview
The business is of a local fiber welding repair shop
<img width="768" height="1024" alt="WhatsApp Image 2026-06-17 at 11 03 36 AM" src="https://github.com/user-attachments/assets/99843415-db69-4d08-97f2-843ebdef9c1c" />

### Business Information:
- Business Name: Rahul Fiber Welding Shop
- Location: Berhampur, Odisha, India
- Industry: Fiber Repair & Welding Services
- Established: 2009
- Service Coverage: Berhampur and nearby areas
- Google Rating: ⭐ 5/5
- Customer Reviews: 100+ Reviews
- Google Maps: [Click here](https://www.google.com/maps/place/rahul+fiber+welding+shop/@19.3081513,84.7924588,17z/data=!3m1!4b1!4m6!3m5!1s0x3a3d5be09b310609:0xaf8c29da9cf2bb04!8m2!3d19.3081513!4d84.7924588!16s%2Fg%2F11s8x3gc3v?entry=ttu&g_ep=EgoyMDI2MDYyNC4wIKXMDSoASAFQAw%3D%3D)
- Google Business Profile: [Click here](https://www.google.com/search?kgmid=/g/11s8x3gc3v&hl=en-IN&q=rahul+fiber+welding+shop&shem=epsdc,ltac,rimspwouoe&shndl=30&source=sh/x/loc/osrp/m1/2&kgs=0baacbe2ace9ce6f&utm_source=epsdc,ltac,rimspwouoe,sh/x/loc/osrp/m1/2)

### Services Offered
Rahul Fiber Welding Shop specializes in repairing damaged fiber products, providing a cost-effective alternative to replacement. The shop repairs a wide variety of products, including:
- Automobile Parts (Cars & Bikes):
Back panel, front panel, side panel, body cover, full body, visor, bumper, mudguard, headlight, nose cover, filter box, tank side cover, petrol tank, dashboard, engine cover, mirror, tail light, seat, silencer cover, steel mudguard and air filter.
- Water storage tanks
- Refrigerator body covers
- Air conditioner body covers
- Water filter body covers
- Mannequins
- Pesticide sprayer tanks
- Cooler body covers
- Plastic dustbins
- Boats
- Bus rooftops
- Fiber roofing sheets
- Heat tanks

### Customer Base
The shop serves a diverse customer base, including:
- Individual customers
- Automobile mechanics and garages
- Showroom (service centres) customers
- Repeat customers
- Customers from Berhampur and nearby areas

### Business Context
Although the shop maintained daily transaction records, there was no structured system to analyze business performance. The owner lacked visibility into key business metrics such as customer trends, revenue, expenses, profitability, repeat customers, and repair demand.
This project transforms 2 months of manually self-collected business data into meaningful insights using Python, enabling the shop owner to make informed, data-driven business decisions.


## 🔨 Business Problem
The shop owner maintained daily transaction records but lacked a structured way to analyze business performance. After discussing with the owner, identified the following quwstions as key business questions and organised them into structured format:

-	How are revenue, expenses, and profit trending across weeks.
-	Which expense categories contribute the most to overall business expenses?
-	How has the profit% changed across different weeks.
-	What is the relationship b/w revenue and profit across different weeks?
-	Which source brings the most customers?
-	What percentage of customers return?
-	List the top 10 valuable and loyal customers?
-	What is the distribution of customers across different customer categories?
-	What proportion of revenue comes from within-city versus outside-city customers?
-	What are the top 7 revenue-generating areas?
-	What is the top 7 frequently repaired parts?
-	What is the revenue distribution across different parts?

## 🧩 Project Objectives
- Transform raw business records into an analysis-ready dataset.
- Perform Exploratory Data Analysis (EDA) using Python.
- Understand customer behavior and business performance.
- Analyze revenue, expenses, profit, and operational trends.
- Identify opportunities to improve business performance through data-driven insights.
- Present findings using clear and effective visualizations.
- Provide actionable recommendations to support better business decisions.

## 📂 Datasets Used
Since, this is a real local business, there were no existing database available. I collected daily business in Excel and organised them into well defined table with standardized columns & cosistent data format
The project uses **four tables of excel**:
- `dim_customer` – Customer details
- `dim_date` – Date-related information   
- `fact_transaction` –Transactional data  
- `fact_expense` – Daily business expenses
  
dim_customer Table<img width="1604" height="695" alt="image" src="https://github.com/user-attachments/assets/23c4a82c-13a9-48ab-9430-9b5efacda6f6" />


dim_date Table<img width="126" height="695" alt="image" src="https://github.com/user-attachments/assets/5e3cb159-d195-4895-8e32-ef8c73a4c99b" />


fact_transaction Table<img width="1206" height="688" alt="image" src="https://github.com/user-attachments/assets/c3b4aae1-615e-4f46-8ad9-525023a25ee8" />


fact_expense Table<img width="690" height="688" alt="image" src="https://github.com/user-attachments/assets/2d669c96-c609-4419-a031-4a1b6761030b" />





## 📥 Data Collection
- Collected two months of real business transaction data
- Recorded the data in four structured Excel files
- Organized customer, transaction, expense, and date information

## 🔍 Data Import & Exploration
- Imported Excel datasets using `pandas.read_excel()`
- Reviewed dataset structure using `head()`, `shape()`, `describe()` and `info()`
- Verified data types and column consistency
- Understood relationships between datasets before merging

## 🧹 Data Cleaning
- Checked data types and corrected them where required. 
- Converted date columns into the appropriate datetime format. 
- Replaced placeholder values (such as "-") with suitable numeric values where necessary. 
- Converted numeric columns using pd.to_numeric() to ensure accurate calculations.

## 🔄 Data Transformation
- Merged the four datasets into a single analysis-ready dataset using `merge()`.
- Created new calculated columns such as Week Number.
- Aggregated data using `groupby()` to generate business-level summaries.
- Calculated key business metrics including Revenue, Expenses, Profit, and Profit %.
- Prepared the final dataset for visualization and exploratory analysis.

## 📊 Exploratory Data Analysis (EDA)
- Performed exploratory data analysis to understand business performance and customer behavior.
- Explored patterns, trends, and relationships within the data.
- Summarized data using aggregation techniques such as `groupby()`.
- Visualized key metrics using Matplotlib and Seaborn.
- Derived actionable insights to support data-driven decision-making.


## 💡 Key Insights
- Customer referrals are the largest acquisition source. 
- The top 10 customers contribute over half of total revenue. 
- Labor costs account for the highest share of expenses.
- Weekly revenue and profit increased by 15%. 
- Returning customers contributed 42% of revenue. 
- Garage referrals generated the highest-value custom

## ⚙️ Tools & Libraries
* Microsoft Excel	Data- collection and storage
* Python Programming language- used to develop the analysis workflow
* Jupyter Notebook-	Interactive development environment
* Pandas-	Data cleaning, transformation, and analysis
* NumPy-	Numerical computations
* Matplotlib-	Data visualization
* Seaborn-	Statistical data visualization


## 🎥 Project Walkthrough 

## 🔗 Connect With Me
- **LinkedIn:** https://www.linkedin.com/in/jyoti-nayak-12884a331/
- **Gmail:** kumarijyotinayak97@gmail.com

## 📌 Conclusion

This project demonstrates how raw business data can be transformed into meaningful insights using Python. By collecting, cleaning, transforming, and analyzing real-world data from a local fiber welding shop, I identified trends in revenue, customer behaviour, expenses, profitability, and business performance.
Using Pandas for data manipulation and Matplotlib and Seaborn for visualization, the analysis answered key business questions and highlighted opportunities to support better decision-making. This project also strengthened my practical skills in data cleaning, data transformation, exploratory data analysis (EDA), data visualization, and business analytics using Python.







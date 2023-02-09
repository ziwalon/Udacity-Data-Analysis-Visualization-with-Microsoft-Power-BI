
# Project Overview

In this project, you'll create a data model and Power BI report for Seven Sages Brewing Company that combines information from all over the company. Your data model will make it possible for the company's CFO to quickly review and analyze what beers sell well and which ones generate the highest profitability.

At the end, you will have applied the key concepts of this course to combine and centralize data that was previously siloed, solving a very common issue facing many companies. More importantly, you'll have a solid foundation to build on when it comes to more complex reporting visualization demands, advanced DAX requirements, or larger data models. No matter how large the data models get as your career progresses, the core principles remain the same.

## Main Steps

Here are the main steps. We'll go over each of these in more detail on the pages that follow.

1. **Source files**. Download and familiarize yourself with the source files provided by SSBC.
2. **Sketch the data model**. Sketch out the data model you intend to build.
3. **Use Get Data**. Use Get Data to load the data from the starter materials into Power BI.
4. **Structure, combine, and clean the data**. Clean and format your data so that it will work well in your data model.
5. **Create your date table**. Create a date table to support time intelligence.
6. **Build relationships between your tables**. Build a relationship from each dimension to the relevant key on the fact table.
7. **Write your measures**. To satisfy the CFO's requirements, we will need to write six measures—to calculate Sales, Cost of Sales and Gross Profit Margin in two different currencies.
8. **Create a report**. Build a basic visual report to display your findings.

### Step 1: Use "Get Data"

Our next step is to use "Get Data" to access the necessary data sources and pull them into Power BI. When reviewing your source data, you'll notice that there are many more files than you want to have in the data model itself. Your job is to merge, append, and otherwise combine the datasets in the most efficient way you can to ensure that they will align with with the data model design you have in mind.

If you're not sure what data model design you want to build, now is an excellent time to review the data available and sketch out your data model, including the keys you'll be able to use to establish relationships between tables.

Ask yourself:

- Which of the data sources will work best as my central fact table?
- Are there any repeating columns that indicate I can or should append similar data into a cohesive singular table?
- Are there any tables that might function as separate dimensions but would perform better merged as a single table?
- If there isn't an obvious join between two tables, is there a logical way I can build one to get access to necessary data?
Beginning with an end in mind will make each step of this process much faster and clearer.

### Step 2: Structure, Combine, and Clean the Data 

As you've learned, most data requires some transformation or cleanup once the data has been loaded into Power BI. Each of these files comes with their own quirks and will require tweaking or corrections. The next three sections will provide some broad-strokes checks to jog your memory, but the details are up to you.

This step is not just formatting cleanup or error handling, however; recall that you will likely need to combine data from different sources when creating a data model, rather than assuming that the structure that each data source arrives in will perfectly meet your needs.

#### Structuring Your Queries and Fields
Correcting the overall structure of how your datasets populate Power Query is a foundational part of developing your data model. Think of this as a collaboration between Power BI and yourself—you both need to be able to recognize which fields are what type and have logical names to be able to work with everything later.

#### Combining data
Often, data needs to be merged, appended, or otherwise combined to meet the desired data model format. This is sometimes done at the initial "get data" loading stage, but can also be done once the files have been made available to combine disparate data sources as needed.

Recall that: "Merge" combines columns between related tables horizontally using one column from each table to define which rows belong together. "Append", conversely, combined tables with the same column headers vertically, and is akin to stapling one printed off table to the bottom of another.

### Step 3: Create Your Date Table

While we'd always prefer to use a date table from the "source" , often you need to build your own. Since Seven Sages runs on a fiscal year, you'll want to build this in Power Query rather than in DAX.

Recall from Lesson 4 that creating a dynamic date table that automatically updates to fit new data is an excellent way to avoid future errors and headaches. You'll want to create a continuous table that covers each full calendar year in the sales data set (starting on January 1st and ending on December 31st. In addition, the table should include:

- Calendar month name and number
- Calendar year
- Fiscal period
- Fiscal year
- Fiscal quarter -Quarter - FY (e.g., Q1 - FY2021)
Seven Sages' Fiscal year begins on October 1st and runs until September 30th. A transaction on Sept 20th 2020 would fall in FY 2020, but a transaction on October 20th would land in FY 2021

### Step 4: Build Relationships Between Tables

### Step 5: Write Your Measures
To satisfy the CFO's requirements, we will need to calculate Sales, Cost of Sales and Gross Profit Margin in two different currencies.

Currency exchange is a tricky (and common) problem you may run into as you grow as a BI analyst. When you face this situation in future, remember to carefully define the requirements on how the currency exchange needs to be reflected in reporting. As we discussed earlier in the course, an exchange rate may be daily, monthly, or run on a rolling average. And it can require more complex data modeling to satisfy reporting needs for multiple currencies. How you handle exchange rates through your data model structure will vary based on the desired end result.

Luckily for us, the CFO provided really clear guidelines. She's only really interested in seeing the Sales total in CAD (Canadian dollars), though she would like it to reflect daily currency exchange rate fluctuations.

When you initially reviewed your starter materials, you may have noticed that the sales record only tracked units sold without applying sales totals. Since the per-unit cost price and sales price values are all in USD, we already have a "standardized" currency to calculate off of and can just apply CAD exchange rates from the currency tables off of that base 1 USD value.

### Step 6: Create a Report
We're on the homes stretch! Next we just need to create a visualization to summarize the output of your data model for the CFO.

The basic version of this report will have two tabs, one summarizing sales by customer and customer type across quarters. The second will simply summarize the percentages of gross profit and unit sales by product.

In both instances, the CFO would like a very brief Executive Summary at the bottom of the tab.
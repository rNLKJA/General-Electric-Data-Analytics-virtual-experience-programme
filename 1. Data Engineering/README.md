# Data Engineering

<https://www.theforage.com/modules/ThbphD5N5WRsd9Mxo/PDif4RapHRZLHb4gT?ref=SfSqDihCcvSen4csq>

## Instruction

<p><a href="https://www.theforage.com?wvideo=q1uryvfab8"><img src="https://embed-ssl.wistia.com/deliveries/3cf886bf45d386e17ec0fc19b80968493bb3432c.jpg?image_play_button_size=2x&amp;image_crop_resized=960x540&amp;image_play_button=1&amp;image_play_button_color=54bbffe0" width="400" height="225" style="width: 400px; height: 225px;"></a></p><p><a href="https://www.theforage.com?wvideo=q1uryvfab8">Task1</a></p>

## Background

At GE Aviation, we use the concept of a “Data Lake”. A Data Lake is a single database instance that contains data from all around Aviation. Everything from financial, delivery (of parts and engines), supplier, engine data, customer data, and so on.

The advantage of a Data Lake is that allows the developer to make a single connection string to the Data Lake, and as long as the developer has permissions to see the data – they are able to immediately start creating data-driven insights in a centralized repository of data.

To simplify this experience, we have put all tables into a single schema (database inside the data lake).

There are 8 datasets that are needed in order to accomplish this task.

![](https://cdn.theforage.com/vinternships/companyassets/ay2tsYxaTif7Nt6z7/AA4Bnq2tJHALwE8cg/Task%201%20image.png)

## Tasks

You have been asked by GE Aviation leadership to create a single data set that combines all the data listed above into a single table.

The data you have been given has sheets related to Flight data (so data relating to the health of the mechanical engine of a plane), Location Data for airports, Manufacturing Data (which relate to various airplane parts), and a manufacturing bill of material (which tells you what engines have been used).

In this final form, we can then use this table to either create a prediction of RUL or visualize the data for easy user consumption. This will be done in task two.

You can complete this task using either Excel OR Tableau

You only need to complete it through one of the methods. For maximum learning, we recommend starting with Excel to get a granular understanding of data analytics, and then for you to try Tableau (as an industry grade tool). If you are a computer science or engineering student, we strongly recommend Tableau.

Before you jump into this task - take a second to read the data glossary so you can have a full understanding of the data you're looking at!

[Data Glossary for this task](https://cdn.theforage.com/vinternships/companyassets/ay2tsYxaTif7Nt6z7/GE%20-%20Task%201%20-%20Glossary.pdf)

### Excel Steps (Beginner)

One way for us to create a single data set is to use excel to merge and join these items.

In this iteration of the task, you are given an excel file, with multiple sheets of data (see below excel - GE Dataset to be combined). Your job is to take these various sheets and create one dataset in "Sheet 1" that joins the datasets.

**Steps:**

In the sheet av_engine_aic_psql create a new column "t24_adjusted" that is the result of the column named t24 + 459.67. Then change the original td4 column to "t24_original", and change "t24_adjusted" to "t24".
The reason we are doing this to only one table, is because this airline stored their t24 column in Rankine, the other airlines kept their temps in a standard format.
This is because one airline stores their dataset in a different format than others
This type of data clean up is a common occurrence when dealing with data sources from various systems.
Find common values in the four "av_engine_data" sheets that allow you merge all of the datasets together
Merge those four items into a sheet

**Definition of done for this task**

- This task is complete when you have one sheet that contains all of the data from the av_engine_data sheets, placed into the same structure
- This task is also complete when your merged sheet has the adjusted td4 field
- You can submit a version of this sheet now!

**Bonus task - EXCEL**

Try doing this extra bit of data clean up after you submit your first attempt!

Now using VLOOKUP or INDEXMATCH find the relationships between the "av_manufacturing_supply_chain_psql" sheet and the "av_bom_manufacturing_psql" and combine them into a seperate sheet called "manufacturing_combined"

💎 Learn how to do a VLOOKUP and INDEXMATCH here!

**Definition of done for this task**

This task is complete when you have two sheets called “manufacturing_combined” as well as the original "av_engine_data"

**Once complete**

Submit the excel file (which have those merged sheets) at the bottom of this page once done!

### Tableau Steps (Intermediate)

One industry standard tool that may help you also generate the right kind of dataset for this task is Tableau. Tableau allows you to visualise and adjust data sets for business intelligence and is used in industry for this purpose.

**Step 1- Get Tableau**

**Step 2 - Download the dataset & upload it into tableau**

**Step 3 - Use Tableau complete your task, then return to this page to upload your findings**

Now in Tableau, your job is to:

1. In the dataset av_engine_aic_psql update the td4 column to the result of t24 + 459.67. You can do this by selecting a column in Tableau, right-clicking it and creating a "Calculated Field".
2. Join all flight tables to consolidate data (The flight tables are the tables with "av_engine_data" included in the name). You can do this in the "Data Source" area of Tableau.
3. Given this information, in Task 2, you will be asked to develop some interesting data dashboards that give you insights about the Flight Data Tables.

Take screenshots of your workings in Tableau showing all the data combined into one data source and upload it below to complete this task!

## Resources

- [GE Dataset to be combined](https://cdn.theforage.com/vinternships/companyassets/ay2tsYxaTif7Nt6z7/GE_Dataset_%20Task1.xlsx)
- [GE Dataset Analytics Data Set (Tableau)](https://cdn.theforage.com/vinternships/companyassets/ay2tsYxaTif7Nt6z7/GE%20Data%20Analytics%20Data%20Set.zip)

- [How to set up an excel datasource in Tableau](https://help.tableau.com/current/pro/desktop/en-us/examples_excel.htm)
- [Free Training Videos by Tableau](https://www.tableau.com/learn/training/20204)
- [Aggregate, Join, or Union Data in Tableau](https://help.tableau.com/current/prep/en-us/prep_combine.htm)

---

<p align=right>@rNLKJA</p>

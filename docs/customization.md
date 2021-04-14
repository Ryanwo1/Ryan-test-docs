---
layout: default
title: Data Analysis
nav_order: 6
---

# Data Analysis
{: .no_toc }


## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---
Microsoft Excel has become one of the most widely used software in all the industries. And data analysis is one of the most important functionalities in Excel which includes sorting, conditional formatting, charts and so on.

## Sorting

### Sort Sheet or sort range

Sort sheet means when we sort a category of values according to a specific pattern, all other correlated values will be moved because of it.

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image1.png?raw=true "starting window")
![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image2.png?raw=true "starting window")

In the original worksheet, all the information was sorted by the “Homeroom” column. However, if we sort the whole sheet again alphabetically by the “Last Name” of people, then not only the order of “Last Name” did change, but information in other columns which is related to this name also moves. 

Sort range means we only sort a part of the cells in a sheet, and it will be convenient when there are a few different tables in the same worksheet. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image3.png?raw=true "starting window")
![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image4.png?raw=true "starting window")

There are more than 1 table in the sheet, so we only want to sort the “Total Orders (by Grade)” on the right. Then after sorting range alphabetically by “Class”, all the cells of “Payment Method” on the left will never be affected. 

## Insturctions
### Sort Sheet

Goal: Sort the whole sheet alphabetically by “Last Name”.

1.Select any cells in the “Last Name” column. For instance, we choose C2 this time.

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image5.png?raw=true "starting window")

2.Find “Data” on the top of the menu, and click the “A-Z” command to rank names from initial A to initial Z. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image6.png?raw=true "starting window")
 
3.The result has been presented below. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image7.png?raw=true "starting window")

### Sort range

Goal: Sort the number of “Orders” increasingly only in table “Total orders (by Grade)”.

1.Select all the values in “Class” and “Orders” columns. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image8.png?raw=true "starting window")

2.Find “Data” on the top of the menu, and click the “sort” command. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image9.png?raw=true "starting window")

3.Click the ![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image10.png?raw=true "starting window") in “sort by” category and choose “Orders”. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image11.png?raw=true "starting window")

4.Choose “Cell values” and “Smallest to Largest” separately. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image12.png?raw=true "starting window")

5.Confirm all your operations by clicking OK to see the result below. 


![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image13.png?raw=true "starting window")

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image14.png?raw=true "starting window")

### Conditional Formatting

Conditional formatting is a functionality which allows users to format cells which meet some specific criteria. Conditional formatting enables users to do the following things. It is able to work as a reminder by asking people to pay attention to some important data. In addition, it can make some big data more visible so that these complicated values can be understood more easily. In this example, we are going to apply conditional formatting rules, so that the percentage of anyone which is greater than 100% is shown in green. 

1.Select all the values in the “Percentage” column.

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image15.png?raw=true "starting window")

2.Click “Home” and find “Conditional formatting”. Then Choose the first “Highlight Cell Rules” -> “Greater Than”.  

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image16.png?raw=true "starting window")

3.Enter “100%” into the blanck in the left under the text “Format cells that are GREATER THAN”. 

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image17.png?raw=true "starting window")

4.Click  in the right blanck after text “with” and find “Green Fill with Dark Green Text”.   

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image18.png?raw=true "starting window")

5.Confirm all the choices by clicking the “OK”, and the final result is shown in below.

![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image19.png?raw=true "starting window")
![starting-window](https://github.com/Ryanwo1/Rykyha/blob/gh-pages/assets/images/data-analysis-image20.png?raw=true "starting window")

Now, you know some basic knowledge about how to analyze data by using Excel. However, the functionalities of sorting and conditional formatting are not limited to the content mentioned above. We can still explore them by ourselves to analyze the data in a more personalized way.  



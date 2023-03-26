
# Project Description

## Introduction

You work as a business intelligence analyst for **Waggle**, a startup that makes smart devices for pets. Recently, Waggle has been thrilled by the success of their new Lapdog device, **a fitness collar that lets owners track their dog’s steps, alerts them when it’s time for a walk, and even repels fleas**! Reviews have been fantastic, sales are growing, and—best of all—the product really works!

This success has led Waggle’s CEO to push for a feline version but there are concerns about its viability. For this reason, the product team distributed 1,000 Lapcat prototypes for field testing. Now, after months of data collection, **you have been tasked with delivering a boardroom-ready Power BI report that tells the story of how the Lapcat data compares to findings from the dog collar Lapdog devices**. You’re excited because your work will be presented at the highest levels of the company and will either help convince the CEO that Lapcat is the next big thing or a costly mistake to be avoided.

### **_Lapdog and Lapcat Logos_** 

![Lapdog and Lapcat Logos](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/marketing_collateral/lapdog_logo_transparent_blue.png) 
### **_Vs._** 
![Lapdog and Lapcat Logos](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/marketing_collateral/lapcat_logo_transparent_pink.png)

### Business Requests:
- The CEO is curious about the following questions:
    1. Did the average daily steps increase for cats wearing the device as they did for dogs?
    2. Were owners of Lapcat devices as satisfied with the product as Lapdog owners?
- The Chief Marketing Officer would like your report to be “on-brand” by including only colors from the Waggle color palette, the Waggle logo, and other approved company logos and icons.
- The product team trusts you to incorporate other visuals and insights as you see fit but is most interested in demographic comparisons between the dogs and cats using Waggle devices as well as any information about the families who own the pets. They would also like slicers to help them filter and explore on their own.

### Resources and Basic Requirements:

A data model has already been provided for you in the Power BI file, as well as a variety of Waggle marketing images and branding guidelines. **Your report should demonstrate best practices in clean layout design and color use, utilize at least 7 different Power BI visualizations, include buttons for navigation between pages and/or bookmarks, and satisfy the business requests stated above.**

### **_Waggle Logo_** 

![Waggle Logo](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/marketing_collateral/waggle_logo_blue.png) 


### Project Steps 
1. Review the included data model and business questions and identify which fields can be used to design metrics that answer the CEO’s questions. (That's all, just understand the data!)
2. Develop one or more visualizations that specifically address the CEO’s questions about whether there was a difference in average daily steps over time between the two devices and how Lapcat owners rated their device compared to Lapdog owners.
3. Address the product team’s request for demographic insights, using each of the following visuals at least once: Bar chart, line chart, donut chart, table/matrix, scatter plot, bubble map, and card.
4. Place your data visualizations and design an appropriate layout that emphasizes the most important findings first, with the CEO's questions answered on the first page, insights about the differences between dogs and cats on the second, and insights about the families who own the pets on the third.
5. In your data visualizations, incorporate the branding elements requested by the Chief Marketing Officer.
6. Please include at least five slicers on each page with at least one example of a drop-down slicer, at least one example of a slider slicer, at least one example of a hierarchy slicer, at least one example of a slicer with “Select All” enabled, and one example of a slicer with the search box enabled.
7. Create at least two bookmark features. One must allow users to dynamically swap one visual out with a different one and another must reset all applied filters on the page.
8. Create buttons that help your users navigate your report. Buttons must respond when users hover over them by changing color or size (or both!).

## First Thing First.

Make sure you have completed all preliminary tasks before starting your report:

- Download and install the latest version of [Power BI Desktop](https://www.microsoft.com/en-us/download/details.aspx?id=58494) on your machine
- Download the provided Waggle marketing collateral attached to the repository
- Download the provided starter.pbix file that contains the Waggle dataset attached to the repository

### **_Waggle Branding Guidelines and color palette_** 

![Waggle Branding Guidelines and color palette](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/marketing_collateral/color_palette.png) 

# My Project

### Understanding the data

The CEO has two questions: 1) whether cats wearing the device had an increase in average daily steps similar to dogs, and 2) whether Lapcat owners were as satisfied with the product as Lapdog owners. The Chief Marketing Officer wants the report to use only approved company branding. The product team wants the report to focus on demographic comparisons between dogs and cats using Waggle devices and information about the families that own the pets. The product team also wants slicers to help them filter and explore the data. The team trusts the writer to add other visuals and insights as needed.

### CEO's Page (Tab 1) 

This report analyzes whether cats wearing the device had an increase in daily steps compared to dogs wearing the device. The report includes a line chart that shows the average daily steps over time for cats and dogs. The chart reveals that dogs wearing the device are more active than cats and that the daily average steps for dogs flat out at about 15 thousand steps while the average for cats fluctuates between 2600 and 2800 steps without showing any significant increases. Based on this data, it is likely that the device for cats will be a flop if rolled out on a wider scale.

Additionally, a bar chart displays the ratings between Lapdog and Lapcat devices as provided by their respective owners. The graph shows that the Lapdog device has an average rating of 4.69 while the Lapcat device has an average rating of 1.64. This indicates that the Lapdog device is much more favorable than the Lapcat device.

The report provides options to filter by pet type, year, rating, and age. The report also adheres to the approved company branding guidelines by using only colors from the Waggle color palette, the Waggle logo, and other approved company logos and icons.

![CEOs Insights Default Page](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/Dashboards/CEOs_Insights_Default_Page.png)

![CEOs Insights Dogs Page](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/Dashboards/CEOs_Insights_Dogs_Page.png)

![CEOs Insights Cats Page](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/Dashboards/CEOs_Insights_Cats_Page.png)

### Pets Insights Page (Tab 2)

This section of the report conducts an in-depth analysis of pets utilizing the devices through the use of a range of graphical displays, such as age-based averages of device ratings and activity levels. The report also incorporates various additional visual aids to effectively communicate key insights.

![Pet_Insights_1](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/Dashboards/Pet_Insights_1.png)

![Pet_Insights_2](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/Dashboards/Pet_Insights_2.png)

### Family Insights Page (Tab 3)

This particular section of the report provides a comprehensive analysis of the pets utilizing the devices from the perspective of pet owners. This includes insights into the specific locations where the devices were purchased, as well as the average household income of the pet owners and annual expenses incurred for their pets. Additionally, the report includes detailed visualizations demonstrating the concentration of device locations.

Overall, these valuable insights equip the CEO of the company with the necessary information to make an informed decision on whether to move forward with the roll-out of the device or explore alternative opportunities.

![Family_Insights](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-2-Power-BI-Report-for-Waggle/Dashboards/Family_Insights.png)



# E-Commerce_Analysis

### Dashboard Link :

## Problem Statement

This dashboard helps the company to  understand their customers better. 
It helps the company know if their customers are satisfied with their services.
Through different customer behaviour, they get to know their improvement area, & thus they can improve their services by identifying these area.
It also lets them know the order status and delivery status, thus since by using this dashboard they can further work on factors responsible for these unwanted cancellations.

### Steps followed 
- Step 0: In e-commerce analysis I have made 3 reports showing different vizualization.

  ## Report - 1 : Customer traffic and yearly trends by different channels

- Step 1 : Load data into Power BI Desktop, one dataset is a csv file and another is xls file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : In the report view, under the view tab, theme was selected.
- Step 6 : Visual filters (Slicers) were added for four fields named "Location", "Gender", "Month Name" & "Year".
- Step 7 : Five card visuals were added to the canvas, representing "Total Revenue","Total Orders","Total Discount","Count of Channel","Count of Location". 
- Step 8 : A column chart was created displaying the Total revenue done by company from the orders made by different gender of customers using different channels.

   - I have used Dax function in power query editor to calculate Total Revenue
     
   - ie Total_Revenue = Sum('Orders Data'[ORDER_TOTAL])
  
- Step 9 : A area chart was created displaying the Total revenue done by the company from the orders made by different customers using different channels 
- Step 10 : A line chart was created displaying the Total revenue done by the company from the orders made by different customers in different years and months

  - Here I have used Dax function in power query editor to calculate Years and Months
    
  - ie Year = YEAR('Orders Data'[ORDER_DATE])
  - Month_Name = Format('Orders Data'[ORDER_DATE],"mmmm")
  
- Step 11 : A pie chart was created displaying the Total orders done by the customers in different years.  

  - Here I have used Dax function in power query editor to calculate Total orders
    
  - ie Total_Orders = Count('Orders Data'[ORDER_NUMBER])
  
- Step 12 : A pie chart was created displaying the Total orders done by the customers by different channels.
- Step 13 : In the report view, alongside the headings of all reports i have created a back button to shuffle between different reports.
  
   # Report Snapshot (Power BI DESKTOP)
   Snap of report 1 : ![Snap_1]()

  ## Report - 2 : Happy customers and Order efficiency based on different channels
     step 1 to step 5 are same as above.
- Step 1 : Visual filters (Slicers) were added for four fields named "Location", "Gender", "Acquired Channel", "Referred other Customer" & "Year".
- Step 2 : Two column charts was created displaying the Count of Customer who referred to other customer and Sum of the Total orders done by the customers based on order status.
- Step 3 : A pie chart was created displaying the Count of customer ID of different customers based on order status.  
- Step 4 : A bar chart was created displaying the Sum of total orders of the customers who referred to other customers.

  # Report Snapshot (Power BI DESKTOP)
  Snap of report 2 : ![Snap_1]()

 ## Report - 3 : Monthly trends and activities in different cities 
   step 1 to step 5 are same as above.
- Step 1 : Visual filters (Slicers) were added for four fields named "Location", "Gender", "Year".
- Step 2 : A line chart was created displaying the Sum of Total orders done by the customers in different Months.
- Step 3 : A pie chart was created displaying the Count of the customers ID of different customers based on different Months.
- Step 4 : A doughnut chart was created displaying the Sum of Total orders done by the customers based on different Locations.
- Step 5 : A bar chart was created displaying the Count of the customers ID of different customers based on different Locations.

  # Report Snapshot (Power BI DESKTOP)
  Snap of report 3 : ![Snap_1]()

# Insights

A Three page report was created on Power BI Desktop.
Following inferences can be drawn from the dashboard;

### [1] Total Revenue of Company  = 22M

   Revenue made by Number of Customers (Male) using app  = 16M

   Revenue made by Number of Customers (Female) using app = 10M

   Revenue made by Number of customers (Male) using website = 18M

   Revenue made by Number of customers (Female) using website = 13M
         
            thus, revenue made by male number of customers are higher.
           
### [2] Total Orders = 30K
     
   Orders made by customers in year 2015  = 2k(6.27%)

   Orders made by customers in year 2016  = 28k(93.73%)

   Orders made by customers using app =  23.3K

   Orders made by customers using website = 26.4K 

            thus, orders made by customers in year 2016 using website are higher.
            
### [3] Sales done by company based on year and months
  
  Highest sales done in which month and year = June , 2016
 
  Lowest sales done in which month and year = November , 2015
      
           thus, sales done in year 2016 is higher than the sales done in year 2015.

 ### [4] Some other insights
 
 ### Location
 
 1.1) Highest orders are placed from Gurgaon = 33.34%
 
 1.2) 2nd highest orders are placed from Chennai = 32.82%
 
 1.3) 3rd highest orders are placed from Banglore = 24.64%

 1.4) Lowest orders are placed from others = 8.59%
         
### Count of customers 

 2.1) Count of customers whose orders are delivered = 96.71%

 2.2) Count of customers whose orders are cancelled = 3.24%

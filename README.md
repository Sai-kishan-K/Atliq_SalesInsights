# Atliq Sales Insights-Dashboard


## Problem Statement

This dashboard helps an organization called AtliQ understand their sales insights on hradware goods better. It helps the company know about their customers and vendors profit and losses through different region, they get to know their improvements over time in each sector of the products, & thus they can get know where the organization needs improvement. It also lets them know the Top 5 customers over revenue & product, thus since by using this dashboard they have identified the insights, they can further work on factors responsible for the decrease in sales.



### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.But there will be some values sales amount in USD 
- Step 5 : So the amounts table is completely converted to INR using the formula 'if currency = 'USD' amount = amount*83'
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Since the data contains various tables, we need insights based on years as well so we extracted only years from 'cy_date' and stored it in seperate column
- Step 8 : Visual filters  were added for better insights on Total revenue and Sales Quantity.

           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
           Although, by default, while calculating average, blank values are ignored.
- Step 10 : A bar chart was also added to the report design area representing the Revenue by each market sectors and amount of sales for the respective markets. 



# Snapshot of Dashboard (Power BI Service)

![Dashboard_snap](https://github.com/user-attachments/assets/65e13e6d-941c-4b6c-a44f-d8588f157910)
 
 # Report Snapshot (Power BI DESKTOP)

![Atliq_dashboard](https://github.com/user-attachments/assets/fd6ad3ec-8e3b-42b0-b169-95cf54e38790)

# Insights

A single page report was created on Power BI Desktop

Following inferences can be drawn from the dashboard;


   Total Revenue  = 984.81 Million

   Total Amount of Sales = 2 Million 

   Top 5 Customers = ElectricalSara Stores, Electricalslytical, Excel Store, Premium Stores, Nixon

   Revenue Trend Over the years which can also been seen for each month for each year.

   


           

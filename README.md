# Power-BI-Paginated-Report


# Creating Parameter
Parameter is to dynamically data filtering, report customisation

  - Go to Power BI Desktop
    - Select for e.g category -> drag and drop in the report view page
    - On the left pane (Filters) -> select Filters on this visual Category and select any data
    - Then go to "OPTiMIZE" tab in top bar
    - Click on "Performance Analyzer"
    - Click Start Recording
    - Refresh Visuals -> You will see the Table
    - Then click Stop
    - Expand the table -> You will see "copy query" -> copy that
   
  - Now Go back to Power BI Report Builder
    - Right click -> Add dataset
    - Give the name "Categorydataset"
    - select "data source" from the dropdown
    - Paste the query which you copied from power bi desktop
    - Click on validate query to make sure it works and click OK

  - Now go to Parameter Folder in the power bi Report builder left pane
    - Incase if there is a default parameter already created -> right click on that particular parameter - select parameter properties
    - Incase if there is no default parameter, then right click on the Parameter folder -> Add Parameter
    - Select "Default values" -> Get values from a query  -> select dataset folder and value field which you just created and then click OK
  
  - Finally Run the report

# Total 
   - Right click on cell -> select Expression
   - select "field dataset"
   - type =SUM( double click on the particular data e.g actual price and then close the parenthesis ) and then click OK
   - Lets do the same for TOTAL -> right click on the above cell -> select expression -> copy the query
   - Right click on the total cell -> select expression -> paste the above copied query -> OK
   - Finally Run
# Formating
 - if click on the table area, it will show tablix
 - if you click on gray area, it will show report properties on the left pane.
 - Also you can right click on the gray area -> select properties -> select the page orientation and paper size etc
 - To enable properties on the left pane, Go to the View tab, check the properties box
 - If you want to add column, select a particular column on the table, right click and select insert column and then select whether to select to insert on the right or left

   
# Expression
  - Right click on the cell
  - select "expression"
  - right after the equal bar , double click on the data  e.g if you want to insert sales price, just double click on that value (e.g = salesprice - budgetprice)
  - Then click OK
  - To change to Currency, Go to HOME table, select currency from dropdown and add the decimal places as per your requirement

To change the font color
  - click on the cell
  - On the Text Box properties on the left, select Font color drop down button
  - select expression
  - Under program flow, select =IIF( enter e.g salesprice>0,"green", "black") and close
    

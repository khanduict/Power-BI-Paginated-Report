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

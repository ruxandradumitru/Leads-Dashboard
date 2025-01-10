I had to recreate a dashboard from Excel to Tableau, by using the database in Microsoft SQL Server. This was for a global E-Learning software company.
Previously I was downloading the raw data from Microsoft Dynamics CRM and I was populating the Excel report and modifying the formulas and design according to the requests coming from Business.
This dashboard was showing the monthly Marketing Qualified Lead numbers for 3 consecutive years, the growth % for each month YoY, as well as the cumulative volume for each year. 
The challenge was for creating a graph in Tableau that compared the Marketing Generated Leads (AQL) to the Marketing Qualified Leads (MQL) and the MQL to the SQL (Sales Qualified Leads). 
I had a single reference for each lead in the database, but with different dates according to the qualification level that it reached and these were appearing in different tables. 
Because of this issue and because I could not use Data Blending (the Tableau version did not incorporate this function at that time), I had to use 'Union All' in the SQL script and then, in Tableau, I used a Bar-in-Bar chart combined with a Graph line. 
Also, I have added a graph with the actual number of orders (number of Won Opportunities), combined with Revenue and Goals. I had to convert the values from different currencies into USD within the SQL script. 
I also incorporated a regional filter in Tableau for all charts/graphs in the dashboard. 
There is a big difference between the revenue figures and the goals shown because the Revenue Data was pulled from the Estimated Revenue Table submitted by the Sales team and not from the actual Invoiced Revenue table (Business decision). 
You may see below the scripts and the dashboard created. Revenue and goal figures have been concealed. 

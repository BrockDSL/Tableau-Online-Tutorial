<img src="tableau-logo.png" alt="Logo" width="150px" hight="150px">

# Introduction to Tableau Online  
A beginners guide to making interactive data visualisations using Tableau Online



### Getting Started  
First things first you will need to download the files that we will be using for this tutorial.  Navigate to each of the links below.  You will be taken to a GitHub page showing the data.  Right click on the "Raw" button at the top right of the data and select "save link as" to save the files to your computer.  
  
[File 1](Order-Contents.csv)  
[File 2](Order-Details.csv)  
  

Next you will need to log in to Tableau Online.  Navigate to the [login page](https://sso.online.tableau.com/public/idp/SSO) and enter your login information.  If you do not have a login you can request a free trial of the full version of Tableau Online [here](https://www.tableau.com/trial/tableau-online).  
  
  
Once you have logged in you should arrive at you Tableau Home Screen.  Your Home screen on Tableau can be changed so to make sure that you are on the correct screen, click on the "Projects" tab.
![Screenshot 1][scrn1]  
  
Now we will create a new project by clicking on the "New Project" button.  In the new project popup enter the title you want to use and a description of the project.  For this example we will use "Shipping Data Analytics" as our project name and will describe it as "Learning to use Tableau is awesome!".  

At this point we will go into the newly made project.  Here we find ourselves on a screen that looks almost exactly like the last one except that by default we will have been moved over to the "Workbooks" tab.  In tableau you can nest projects in order to maintain a clean hierarchy of data.  
  
Now that we have a project to contain our data lets click on the "New Workbook" button so that we can start working with our data!
  
### Working with our data

When you open a new workbook you will be presented with the "connect to data" page.  Here you can either drag files into your workbook or upload them from your computer.  It is easiest if you select all of your data and drag/open it into the workbook all at once.  
  
![Screenshot 2][scrn2] 

When bringing data into Tableau you will often be using multiple files.  If these files share a common field (known as a "table key") you can use that field to connect your data and make it much easier to work with.  In this example both of our files have an "Order ID#" field that will be our key.  
  
Once you have added your data you will either be taken directly to the worksheet area (if you added only 1 data source) or to the Data Source area (if you added multiple data sources).  In this tutorial you should be at the Data Source area.  If not you can navigate there using the "Data Source" tab at the bottom left of the page.  This is the area where you can make connections between data sources to tie their data together.  Drag the Order-Contents.csv file from the files list on the right into the tables area.  You will see that Tableau has read the file and guessed that the first row of our table is the headers and has displayed them below.  You can get a full preview by clicking the "Update Now" button.  
  
Next we will drag the Order-Details.csv file into the tables area.  Tableau notices right away that both tables have an Order ID# column that has points that match up with each other so it automatically makes a connection between the two files.  Now the data from both files is connected so that we can see for example how order #1 was sold at $8,134.00 per unit (from the Order contents file) to Reims Collectables in France (from the Order Details file).  You can see what field was used to connect the data by hovering over the connecting joint.

![Screenshot 3][scrn3]  
  
Now that we have brought in and connected our data it is time to start working with it to make useful visualizations!  Click on the "Sheet1" tab in the bottom left corner to move to our first worksheet.  Each worksheet represents one visualisation that we can combine into a dashboard later.  
  
On the left side of worksheet you will see your data menu.  Here you can select which data you will use in your visualisation.  The menu is split into Dimensions, which are _**usually**_ used to define your columns and rows, and Measures, which _**usually**_ are used to define the values in a visualisation.  We say usually because in tableau almost any data can be used in any part of a visualisation.  Some measures can even be turned into dimensions and vice versa!  
  
Adding data to a visualisation is as easy as dragging and dropping a piece of data from the menu into one of six  locations on the worksheet.  For now we will focus on the main four areas used to make visualisations.  The image below shows these four areas.  
  
![Screenshot 4][scrn4]  
  
Lets try it out by dragging "Product Type" from the dimensions menu into the visualisation area.  Tableau automatically decides that this data would be best represented as rows so it puts the pill (the colored oval representing this piece of data) into the Rows shelf.  Tableau has taken each unique value from the Product Type data and turned it into a row header in a table.  You will also see that the next column in the table has no title and is filled with "Abc".  This is how tableau tells us that more information is required to make this kind of visualisation.  Now lets add a value to this table.  To do this we will drag "Quantity Ordered" from Measures into the empty space at the bottom of the Marks box.  Nothing has changed aside from a green pill called "SUM(Quantity Ordered)" now sits at the bottom of the Marks box.  This is because we have to tell Tableau that this data should be represented in the visualisation as text.  we do this by clicking the little pile of dots beside the pill and selecting that we want this pills data to be represented as text.  Tada!  Now we have our first visualisation of our data.  
  
Tables are very useful for people who like numbers but sometimes you need to present your data in a more compelling way.  That is where the true power of Tableau comes in.  Drag your green pill from the Marks box up into the Columns shelf.  Tableau recognises that the best way to display this data has changed and adjusts accordingly by switching from a table to a bar graph.  Now we can see from a quick glance that Classic Cars are by far the most ordered product and Trains are the least.  To see more specific information you can hover over individual bars in the graph to view the tooltip which contains the details for that data.  To polish our visualisation even further we can sort our graph by hovering over the lable on the bottom (Quantity Ordered) and clicking once on the sort icon that appears there.  Now our graph is sorted in descending order.  To switch to Ascending we click the sort button again and to remove the sort we click it a third time.  
  
![Screenshot 5][scrn5]
  
Now we have a beautiful and compelling visualisation showing us the total number of each product type that was ordered.  As great as this is, we need to remember that our data spans three years.  What if we wanted to see data for just one year?  This is where the filters box comes in.  Any data we have can be used as a filter to narrow the focus of our visualisation.  We want to see specific years so lets drag "Date of Order" from dimensions over to the Filters box (right above the Marks box).  You will now see a filter appear on the right of the visualisation.  Here you can select which years data you want to display!  Try unchecking the boxes to see how the graph changes.
  
Now that we know how to input data into our visualisations lets see what other forms it can take.  In the top right corner you will see the "Show Me" button.  This opens a menu for changing which type of visualisation you are using to represent your data.  As you hover over each type you can see what kind of data is needed to use that visualization.  Click on one that you like and see how your data looks in a different form.  
  
Take some time to try out different combinations of data and visualisations.  
  
![Screenshot 6][scrn6]















[scrn1]: tableau-scrn1.png  
[scrn2]: tableau-scrn2.png  
[scrn3]: tableau-scrn3.png  
[scrn4]: tableau-scrn4.png  
[scrn5]: tableau-scrn5.png  
[scrn6]: tableau-scrn6.png  
[scrn7]: tableau-scrn7.png  
[scrn8]: tableau-scrn8.png  
[scrn9]: tableau-scrn9.png  
[scrn10]: tableau-scrn10.png  

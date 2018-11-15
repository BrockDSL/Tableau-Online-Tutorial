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
  
Now that we have brought in and connected our data it is time to start working with it to make useful visualizations!  Click on the "Sheet1" tab in the bottom left corner to move to our first worksheet.  Each worksheet represents one visualisation that we can the combine into a dashboard later.



















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

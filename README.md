<img src="tableau-logo.png" alt="Logo" width="150px" hight="150px">

# Introduction to Tableau Online  
A beginners guide to making interactive data visualisations using Tableau Online



### Getting Started  
First things first you will need to download the files that we will be using for this tutorial.  Navigate to each of the links below.  You will be taken to a GitHub page showing the data.  Right click on the "Raw" or "Download" button at the top right of the data and select "save link as" to save the files to your computer.  
  
[File 1](Order-Contents.csv)  
[File 2](Order-Details.csv)  
[File 3](Sample-Image.png)  
  

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
  
Now we have a beautiful and compelling visualisation showing us the total number of each product type that was ordered.  As great as this is, we need to remember that our data spans three years.  What if we wanted to see data for just one year?  This is where the filters box comes in.  Any data we have can be used as a filter to narrow the focus of our visualisation.  We want to see specific years so lets drag "Date of Order" from dimensions over to the Filters box (right above the Marks box).  You will now see a filter appear on the right of the visualisation.  Here you can select which years data you want to display!  Try unchecking the boxes to see how the graph changes.  If you want to get even more detailed you can add another instance of "Date of Order" to the filter box.  Now click the down arrow on the new pill and select month to add the new filter to the right of your page.
  
Now that we know how to input data into our visualisations lets see what other forms it can take.  In the top right corner you will see the "Show Me" button.  This opens a menu for changing which type of visualisation you are using to represent your data.  As you hover over each type you can see what kind of data is needed to use that visualization.  Click on one that you like and see how your data looks in a different form.  
  
Take some time to try out different combinations of data and visualisations.  
  
![Screenshot 7][scrn7]  
  
You will notice that beside each piece of data in the menu there is a symbol that represents what kind of data it is.  Tableau has assigned a type that it thinks best suits each piece of data.  These types are important for working with certain visualisations.  In the "Show Me" menu when you hover over certain visualisations it will show that a specific type of data is required to use it.  For example the Map visualisations require geo data.  If you want to change the type on a piece of data click on the down arrow that appears when you hover over it.  Go down to "Change Data Type" and select the data's new type.  Keep in mind the data that you are changing the type of.  Just because you changed you list of products into geo data does not mean that Tableau will be able to make a map out of it.  You can also change data from being a dimension to being a measure by clicking its down arrow and selecting "Convert to Measure/Dimension".  This can be useful if you want the count of values in a piece of data as opposed to the value's themselves.


### Sheets and Dashboards

Now that you can make visualisations you need to know how to show them off.  At the bottom left of the visualisation area you will see the buttons to add new sheets, dashboards and stories.  Each sheet can contain one visualisation.  For this example lets make three sheets with three different visualisations on them.  Rename your sheets to something representative of what the visualisation contains by right clicking on the sheet in the bottom menu and selecting "Rename".  Next we will create a dashboard using the "New Dashboard" button on the bottom bar.  A dashboard lets you display and arrange your visualisations in a powerful interactive display.  
  
To add a visualisation to your dashboard, drag one of your sheets from the menu on the left into the dashboard.  
Tableau will automatically adjust it so that it fills the page.  drag the other two visualisations into the dashboard.  Tableau will adjust each piece to fit the space.  This can cause problems with some visualisation types.  If you are unhappy with how Tableau automatically aranges your visualisations you can move them manually by selecting each piece, clicking the down arrow at the top right, and selecting "floating".  This will remove that piece from Tableaus formatting and allow you to move your visualisations around freely by dragging the bar at the top of the items box.  Alternatively you can make all sheets added to the dashboard floating from the start by selecting the "floating" option near the bottom of the left menu before adding any sheets.

![Screenshot 8][scrn8]  
  
  
![Screenshot 9][scrn9]
  
You will notice that like on your worksheets, clicking on differents data on the dashboard highlights that data on that particular visualisation and clicking again on the same data removes the highlight.  We can expand on this functionality by selecting one of our visualisations and clicking on the "Use as Filter" icon.  Now when you select a piece of data from that visualisation it will alter all other visualisations on that dashboard to show only the data related to what you have selected.  
  
![Screenshot 10][scrn10]  

Lets look at customizing a dashboard further.  Just above the "Tiled" and "Floating" buttons you will see a selection of objects that you can use to make your dashboard mor functional and visually apealing.  By clicking and dragging one of these objects onto your visualisation you can add images, text, windows containing web pages, and buttons connecting to other dashboards, sheets and stories.  Lets remove our Orders Per Month visualisation from our dashboard to make some room.  To remove an object or visualisation from your dashboard, select it and click the x in the top right corner.  
  
Now lets add an image to use as a background for our dashboard.  Drag the image object from the menu onto the dashboard.  In the window that pops up select the sample image you downloaded at the beginning of this tutorial and then click ok.  Now resize the image to fit the entire dashboard.  Here you will see that the image has covered everything else that we had on our dashboard.  To fix this fo to the drop down arrow for the image, go to floating order, and select send to back.  This will put the image behind everything else on the dashboard.  Keep this in mind when creating a dashboard using floating objects.  
  
![Screenshot 11][scrn11]  
  
Next let us add some text to our dashboard.  We are going to want to share this with people who may not be familiar with what we are doing so lets add a brief description of our data and instructions on how to interact with it.  Drag the text object onto the dashboard and write some helpful text.  
  
Now we have a nice helpful visualisation with a nice description but what about the Orders per Month?  We could add it to this page but that might end up looking a bit cluttered.  Instead we will make another dashboard and add a button that lets us switch back and forth between the two.  When using multiple dashboards for the same data it is a good idea to maintain a consitant formatting.  We could build the new dashboard from the ground up but it is much easier to copy our current dashboard and then alter it.  To do this, right click on the current dashboard at the bottom of the page and select "Duplicate".  We now have two copies of the same dashboard.  For this tutorial we will rename our new dashboard as "Dashboard 2".  Now lets delete the Total Product Numbers visualisation from our new dashboard and add in the Orders per Month.  Lets also change the text to reflect the new data represented on this dashboard.  To do this, either click the down arrow for the test object and select edit text or double click on the text object.  So now we have two nice clean dashboards that we can show off but to make for easier navigation between the two lets add a button to each.  Drag the button object from the menu onto the dashboard.  Click the down arrow on the button and select "Edit Button".  Here we will change the destination to our other dashboard using the drop down menu and then we will write either "Next Page" or "Previous Page" as the tooltip.  You can also add an image to the buttons if you want to customize them more.  

Now is a good time to **save your progress**.  Saving frequently is a good habit to get into.  Save by either going to the file tab and clicking "Save" or by clicking on the save icon.
  
![Screenshot 12][scrn12]  
  
Now for the fun part!  Lets close this workbook and go back to tableau online.  Click on the views tab.  Here we can see all of our hard work!  Lets hover over Dashboard 1 and then click the "View" button that appears.  Welcome to your dashboard!  In view mode you can interact with your visualisations the same as you could in editing mode except you can't change anything.  Since we made Customers per country our filter clicking on a country will still alter our data.  Also now that we are in view mode our button takes us back and forth between Dashboard 1 and Dashboard 2.  
  
Now let's go back into editing mode and look at one more tool.  
  
![Screenshot 14][scrn14]  
  
  
### Stories  

Stories are interactive slideshows that let you present data visualisations in an order that suits your needs.  To create a new story, click on the "New Story" button on the bottom bar.  To make a quick and simple story, double click on one of you sheets in the menu to add it to the story and then click in the caption box at the top and name the page sometheing relevant to the visualisation it contains.  Repeat this for your other two sheets and you should have a simple story like the one below.  
  
![Screenshot 15][scrn15]  
  
Stories can also be made out of dashboards although buttons do not work in stories.  Stories are the best option for displaying visualisations in a presentation setting where you have a flow of information or a point that you are trying to make with the data.  Using dashboards on their own can be a better option when you are giving the information to someone else to look at and you want them to be able to move around the dat freely.  
  
Think about who your visualisations are for when you are deciding how to present them.  
  







[scrn1]: tableau-scrn1.png  
[scrn2]: tableau-scrn2.png  
[scrn3]: tableau-scrn3.png  
[scrn4]: tableau-scrn4.png  
[scrn5]: tableau-scrn5.png    
[scrn7]: tableau-scrn7.png  
[scrn8]: tableau-scrn8.png  
[scrn9]: tableau-scrn9.png  
[scrn10]: tableau-scrn10.png 
[scrn11]: tableau-scrn11.png 
[scrn12]: tableau-scrn12.png 
[scrn14]: tableau-scrn14.png 
[scrn15]: tableau-scrn15.png 
[scrn16]: tableau-scrn16.png 

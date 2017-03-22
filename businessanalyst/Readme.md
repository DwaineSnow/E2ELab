# Hands on Lab - Business Analyst
[<img src="https://github.com/WatsonDataPlatform/E2ELab/blob/master/Media/DataDiscovery.png">](https://github.com/ibmdataworks/datafirst/tree/master/businessanalyst/)

Perform these hands-on exercises using guided exploration capabilities with IBM Watson Analytics platform on customer transaction data to uncover unique insights about product affinities.
 

# Hands on Exercises...


1.  Logon to Watson Analytics by going to page “watsonanalytics.com” on a browser and clicking on “SIGN IN” text on the top right. 

 [<img src="https://github.com/WatsonDataPlatform/E2ELab/blob/master/Media/WatsonASignon.png">](https://github.com/WatsonDataPlatform/E2ELab/businessanalyst)

2.  If you completed the [Data Engineer Lab](https://github.com/WatsonDataPlatform/E2ELab/tree/master/dataengineer/)you should have the "Great Outdoor Customer Orders.csv" file in your "Personal" folder as shown in the image below. If this file does not exist or you do not wish to complete the Data Engineer lab, proceed to Step 3, otherwise move to Step 4. 

3. Download this file <https://github.com/WatsonDataPlatform/E2ELab/blob/master/GettingStarted/Great%20Outdoor%20Customer%20Orders.xlsx> to a local directory. Click on “+ New data” button towards the top left and choose "Local file". Select your file and choose import. 

 > <img src="./media/image9.png" />

3.  You should now be able to read in a spreadsheet “Great Outdoor Customer Orders.xlsx” that you can download from the Github link: <https://github.com/ibmdataworks/sigmo-demos/tree/master/business-analyst>
    Click on “Local file” to import the dataset into Watson Analytics.
    
 > <img src="./media/image10.png" width="360" height="175" />

4.  You can now either drag and drop the spreadsheet or click on “Browse” to select the file from the folder where you downloaded the dataset from Github.

 > <img src="./media/image11.png" width="360" height="175" />

5.  Next, you should see an icon for the file on the screen and now click on “Import” button on bottom right to upload the spreadsheet to Watson Analytics.

 > <img src="./media/image12.png" width="359" height="204" />

6.  In less than a minute (usually within 30 seconds), the input file is uploaded and processed and shows up as an entry in the Personal folder as shown below. Watson Analytics processes the file to measure its usefulness for analytics and computes a data quality score. The data quality score (77% for this file) is computed as an average of the score of all fields and is influenced by missing values, constant values, imbalance (skews and outliers). To read more about data loading and data quality, please check out: <https://community.watsonanalytics.com/discussions/storage/attachments/816-watson-analytics-intro-to-data-v-2-1.pdf>

 > <img src="./media/image13.png" width="358" height="211" />

7.  You are now all set to start looking at the interesting insights Watson Analytics automatically finds from the data. Just click on the dataset and you’ll be taken to a screen labelled as “New Discovery Set” as shown below. As “Starting points”, 6 different visualizations are automatically recommended for you to explore (you can click on “Show Next” on the top right to see the next set of guided visualizations), but you can create your own visualization selecting from the 20 different chart types in the bottom of the screen. You also have an option to type in a natural language question on the top and Watson Analytics will suggest an appropriate visualization that likely answers that question! 
 > <img src="./media/image14.png" width="359" height="195" />

8.  Let’s scroll back to the top and type in a question “Show the breakdown of Transactions by Product Line and Product Type” and hit enter. You will automatically be provided a set of starting points starting with the most relevant visualization that helps answer your question! Let’s click on the tree map on the top left (the first visualization listed as “Most relevant” under “Starting points”).

 > <img src="./media/image15.png" width="363" height="141" />

9.  Since each row of the spreadsheet is a customer transaction, the size of the rectangles in the Treemap represents the number of transaction for each product type such as “Tents”, “Sleeping Bags”, “Eyewear” etc. We can clearly see that most popular item for Great Outdoors is “Eyewear” and if you hover your mouse over that brown rectangle under “Personal Accessories”, it tells you that there were a total of 8,264 transactions (out of a total of 62K transactions) for “Eyewear”! The next best selling items in terms of total volume are “Tents” and then “Sleeping Bags”.

 > <img src="./media/image16.png" width="358" height="202" />

10. Several other automatically generated “Discoveries” are drawn on the right, but let’s click on the “x” button to close that pane, so as to lay out the Treemap across the entire screen to better visualize the chart. Now, let’s add a field to the “Multiplier” data slot as highlighted on the bottom right by clicking on it and then selecting “Gender” from the pulldown list.

 > <img src="./media/image17.png" width="361" height="202" />

11. On the text box that pops up, make sure to click on arrow to the right of “Multiplier Mode” and select “Vertical”. This will lay out the Treemaps for Females and Males, one below the other (versus the default “Horizontal” option, which is next to each other). This helps better use the screen space to see the Treemap more clearly for each Gender and observe the similarities and differences.

 > <img src="./media/image18.png" width="358" height="195" />

12. Now comparing the Treemaps for the Women and Men respectively, we can clearly see that the most popular item for Women is “Eyewear”, whereas for Men, it is “Tents”! In the “Camping Equipment” category, Women buy more “Sleeping Bags” and then “Cooking Gear”.

 > <img src="./media/image19.png" width="360" height="202" />

13. Let’s now add a title to this visualization by clicking on “Untitled 1” on the tab to the top left and then click on the pencil icon as shown below to type in a title “Product Type vs Gender”.

 > <img src="./media/image20.png" width="359" height="201" />

14. We will create a new visualization now to see the correlation of Age and Gender to Product Line. Click on the “+” button to the right of the title tab of the visualization you just created as shown below:

 > <img src="./media/image21.png" width="359" height="202" />

15. You will be prompted with 6 “Starting points” again and instead of typing in a natural language question (you can type on the text box on the top left “How do the Transactions compare by Age and Product Line”) , let’s create this new visualization by scrolling to the bottom and under “Create your own visualization”, pick the chart titled as “Bar” under “Comparison”. There are 20 different chart options categorized as “Comparison”, “Parts to whole”, “Trend and forecast”, “Relationships”, “Tables and Summary”, “Predictive …” and “Geospatial”.

 > <img src="./media/image22.png" width="359" height="98" />

16. First, dismiss the “Discoveries’ pane on the right by clicking on the “x”, so as get more space to draw out the bar chart. You will see a sample “Bar Chart” and you have to now pick fields for the categories, “Bars”, “Length”, “Color” and “Multiplier”, as shown on the bottom of the chart as below:

 > <img src="./media/image23.png" width="358" height="202" />

17. Drag and drop “Age”, “Transactions” and “Product Line” on “Bars”, “Length” and “Color” data slots respectively.

 > <img src="./media/image24.png" width="358" height="201" />

18. Now click on “Format”, expand “Variations” and perform the following - select “Stacked” and de-select “Swap Axis”. That enables your bar chart to be stacked and presented in a horizontal fashion and enhances the overall visibility of the visualization.

 > <img src="./media/image25.png" width="359" height="202" />

19. Just drag and drop “Gender” from the data tray below to the “Multiplier” data slot.

 > <img src="./media/image26.png" width="361" height="195" />

20. As you compare these, you’ll notice that Females below 30 years of age buy more “Personal Accessories” (shown in purple) and those between 30 and 48 buy more “Camping Equipment” (shown in blue).

 > <img src="./media/image27.png" width="361" height="196" />

21. As for the Males below age 44, they mostly buy “Camping Equipment” (shown in blue) and those older buy “Golf Equipment” (shown in green).
 > <img src="./media/image28.png" width="361" height="196" />

22. You can now rename this tab as “Product Line vs Age and Gender” and save the “New discovery set” you just created by clicking on the “floppy disk” icon <embed src="./media/image29.emf" width="24" height="20" /> and selecting “Save as”, as shown below.

 > <img src="./media/image30.png" width="641" height="116" />

23. On the “Save as” text box that pops up, type “Great Outdoors Customer Order Insights” on the top left and save it in the “Personal” folder (only option available by default, unless you create new folders yourself) by clicking on the “Save” push button on the bottom right.

 > <embed src="./media/image31.emf" width="284" height="266" />

24. We will create one last visualization that will show us the attributes that drive “Product Line”. Click on the “+” and type a question “What drives Product Line” on the top left as shown below and hit enter.
    Watson Analytics returns with 6 resulting insights for you to choose from. Click on the most relevant (top left) Spiral Visualization as shown below.
    
 > <img src="./media/image32.png" width="643" height="228" />

25. Click on ‘View more’ to see the entire list of factors arranged in order of their predictive strengths. You should see the top predictor as “Product Type” with 100% strength (since each Product Line has a set of unique Product Types) right at the center of the bulls-eye and then the next relevant attributes are “Profession and Gender” and “Professional and Age” respectively, each with 50% predictive strength. Click on the “Untitled 1” label for this discovery on the tab on the top right and then click on the “pencil” icon and type in the label “Drivers of Product Line”. You should now see the discovery as below:

 > <img src="./media/image33.png" width="358" height="201" />

26. The predictive insight gleaned from the “Spiral” chart says a Data Scientist can explore building machine learning models such as a “Decision Tree” using the same data with the “Data Science Experience” (DSX) too. There’s a separate lab exercise for the Data Scientist that does exactly that and you’re welcome to try that next!

27. Congratulations, you’re done with the lab exercise!


## Before You Begin

The "Watson Data Platform" labs are done using the IBM cloud. They use a set of fully managed cloud data services; Cloudant, dashDB for Analytics and Object Storage to persist data and Data Connect to ingest data. These services are available in Bluemix, IBM’s cloud platform. They also use Watson Analytics, IBM’s smart data discovery service on the cloud and the IBM Data Science Experience, an interactive, collaborative, cloud-based environment where data scientists can use multiple tools to activate their insights. Lastly, several of the labs require that you download a few files that are used as source datasets and to assist in building an application.

## Workflow

On the following pages are a series of steps you will perform before you do any of the labs. Each step outlines an easy to follow set of instructions that will walk you through preparing your IBM cloud environment so you can do any of the labs you choose. It is a serial process so it’s important that you follow each step in sequence and do not deviate from the workflow or skip any steps in the process.

Step | Description
------------ | -------------
1 | Download the Lab Files
2 | Create a Bluemix Account
3 | Create the Watson Data Platform lab services
4 | Create the Watson Data Platform lab application
5 | Create a Watson Analytics Account

## Step 1: Download the Lab Files

**Download** the Great Outdoor Customer Orders CSV file to your workstation. This file is used in the Data Engineering, Business Analysis and Data Science labs. 

### [Click Here to Download the "Great Outdoor Customer Orders.csv" file](https://github.com/WatsonDataPlatform/E2ELab/blob/master/GettingStarted/Great%20Outdoor%20Customer%20Orders.csv)

**Download** the nodejsDashboard Zip file to your workstation. This file is used in the Application Development lab.

### [Click Here to Download the "nodejsDashboard.zip" file](https://github.com/WatsonDataPlatform/E2ELab/blob/master/GettingStarted/nodejsDashboard.zip)

**Download** the Lab-DSX-ML Zip file to your workstation. This file is used in the Data Science lab.

### [Click Here to Download the "Lab-DSX-ML.zip" file](https://github.com/WatsonDataPlatform/E2ELab/blob/master/GettingStarted/Lab-DSX-ML.zip)

## Step 2: Create a Bluemix Account

You will need a Bluemix account. Follow the instructions in one of the sections below depending on whether or not you have a Bluemix account.

## If you alredy have a Bluemix account...

### Log Into Bluemix 

### [Click Here to Login to Bluemix](https://console.ng.bluemix.net/)

> **Note** - The URL for Bluemix is https://console.ng.bluemix.net

<img src="./media/Step2-image-01.png"/>

1. **Select** the "Log In" button. When prompted, enter your Bluemix ID and password.

### Create a Bluemix Space

<img src="./media/Step2-image-02.png"/>  

1. **Select** the Account information area in the top right corner of your Bluemix account home page.
2. **Select** the "Create a Space" link next to “Manage Organizations” below the Space drop down list box.

  <img src="./media/Step2-image-03.png"/>

3. **Enter** “Watson Data Platform” (without quotes) for the space name.  
4. **Select** the “Create” button.  

> The new space will be created and you will be placed into it. You should now see, in the top right corner, that you are in the “Watson Data Platform” space in your Bluemix organization. You will use this space to house the Watson Data Platform Lab services and application.

**Proceed to Step 3**

## If you don't have a Bluemix account...

### [Click Here to Register for a Bluemix Account](https://console.ng.bluemix.net/registration/)

<img src="./media/Step2-image-04.png"/>

**Enter** the required information *(required fields are marked with an asterick)* on the right side panel.

<img src="./media/Step2-image-05.png"/>

1. **Seletct** the "I'm not a bot" check box.

<img src="./media/Step2-image-06.png"/>

> **Note** - You may be asked to verify multiple images. Select the Skip or Next button as instructed until you get to a screen (as shown above) with a Verify button.

2. **Select** the images you are instructed to select. For instance, Select all squares with street signs. 
3. **Select** the "Verify" button.

<img src="./media/Step2-image-07.png"/>

4. **Review** and check or uncheck the options to be kept informed of products, services and offerings from IBM.
5. **Select** the "Create Account" button when it is enabled for selection.

<img src="./media/Step2-image-08.png"/>

A page will appear notifying you to check your email to complete your registraion. Check the email account that you supplied to register for your Bluemix account and open the email.

<img src="./media/Step2-image-09.png"/>

6. **Select** the “Confirm your account” link.

<img src="./media/Step2-image-10.png"/>

You will be taken to a web page confirming that you sucessfully signed up for Bluemix and that it is now activated.

7. **Click** on the "Log in" link to log into your new Bluemix account.

<img src="./media/Step2-image-11.png"/>

8. **Select** the checkbox to agree to the terms and conditions.
9. **Select** the “Continue” button.

> **Note** - I have redacted my email address on some screen shots to protect my identity, yours will be visible.

<img src="./media/Step2-image-12.png"/>

10. **Click** on the email address suggestion for an organization name. It will be filled in for you as your organization name.
11. **Select** the “Create” button.

<img src="./media/Step2-image-13.png"/>

12. **Enter** “Watson Data Platform" (without quotes) as your Bluemix space name.
13. **Select** the "Create" button.

<img src="./media/Step2-image-14.png"/>

14. **Select** the "I'm Ready" button.

## Step 3: Create the Watson Data Platform Lab Services

<img src="./media/Step3-image-01.png" />

1. **Select** the "Catalog" menu at the top of the Bluemix home page.

<img src="./media/Step3-image-02.png" />

2. **Enter** "data connect" (without quotes) in the catalog search area.  
3. **Click on** the “Data Connect” service.  

<img src="./media/Step3-image-03.png" />

4. **Enter** "WDP Lab Data Connect” (without quotes) for the Service name.  
5. **Enter** “WDP Lab Data Connect” (without quotes) for the Credential name.  
6. **Select** the the "Create" button. The service will be created and the launch page is displayed.

<img src="./media/Step3-image-04.png" />

1. **Select** the "Catalog" menu at the top of the Bluemix home page.

<img src="./media/Step3-image-05.png" />

2. **Enter** "cloudant" (without quotes) in the catalog search area.  
3. **Click on** the “Cloudant NoSQL DB” service.  

<img src="./media/Step3-image-06.png" />

4. **Enter** "WDP Lab Cloudant NoSQL DB” (without quotes) for the Service name.  
5. **Enter** “WDP Lab Cloudant NoSQL DB” (without quotes) for the Credential name.  
6. **Select** the the "Create" button. The service will be created and the launch page is displayed.

<img src="./media/Step3-image-07.png" />

1. **Select** the "Catalog" menu at the top of the Bluemix home page.

<img src="./media/Step3-image-08.png" />

2. **Enter** "dashdb" (without quotes) in the catalog search area.  
3. **Click on** the “dashDB for Analytics” service.  

<img src="./media/Step3-image-09.png" />

4. **Enter** "WDP Lab dashDB for Analytics” (without quotes) for the Service name.   
5. **Select** the the "Create" button. The service will be created and the launch page is displayed.

<img src="./media/Step3-image-10.png" />

6. **Select** the "Service Credentials” tab from the dashDB for Analytics launch page.   
7. **Select** the the "New Credential +" button.

<img src="./media/Step3-image-11.png" />

8. **Enter** "WDP Lab dashDB for Analytics” (without quotes) for the Credential name.   
9. **Select** the the "Add" button. The service credentials will be created.

<img src="./media/Step3-image-12.png" />

10. **Select** the "View credentials v" down arrow to view the newly created credentials.

> **Note** - These are the WDP Lab dashDB service credentials you will need to access the dashDB service in the Data Engineering and Data Science labs. Remember how to get back to this area of the service. I have redacted my password,  to protect my identity, yours will be visible.

<img src="./media/Step3-image-13.png" />

1. **Select** the "Catalog" menu at the top of the Bluemix home page.

<img src="./media/Step3-image-14.png" />

2. **Enter** "apache spark" (without quotes) in the catalog search area.  
3. **Click on** the “Apache Spark” service.  

<img src="./media/Step3-image-15.png" />

4. **Enter** "WDP Lab Apache Spark” (without quotes) for the Service name.
5. **Enter** “WDP Lab Apache Spark” (without quotes) for the Credential name. 
5. **Select** the "Create" button. The service will be created and the launch page is displayed.

<img src="./media/Step3-image-16.png" />

1. **Select** the "Catalog" menu at the top of the Bluemix home page.

<img src="./media/Step3-image-17.png" />

2. **Enter** "cloud data store" (without quotes) in the catalog search area.  
3. **Click on** the “Object Storage” service.  

<img src="./media/Step3-image-18.png" />

4. **Enter** "WDP Lab Object Storage” (without quotes) for the Service name.
5. **Scroll down** the service page to the Pricing area.

<img src="./media/Step3-image-19.png" />

6. **Select** the "Free" service plan.
7. **Select** the "Create" button. You receive a message that the service is being created and that it may take a few minutes. The message will disappear and you will be taken to the services dashboard of your Bluemix account.

<img src="./media/Step3-image-20.png" />

> **Note** - You should have 5 services in your services dashboard. These are the services that will be used by the Watson Data Platform labs; Data Engineering, Business Analytics, Data Science and Application Development.

## Step 4: Create the Watson Data Platform Lab Application

<img src="./media/Step4-image-01.png" />

1. **Select** the "Catalog" menu at the top of the Bluemix home page.

<img src="./media/Step4-image-02.png" />

2. **Enter** "cloud foundry" (without quotes) in the catalog search area.  
3. **Click on** the “SDK for Node.js" Application.

<img src="./media/Step4-image-03.png" />

4. **Enter** "WDP Lab Your Name Application” (without quotes), with Your Name equal to your First and Last Name. The Host name will be filled in automatically for you with dashed in place of spaces.

> Notice that my application name is "WDP Lab Rick Buglio Application" with a Host Name of "WDP-Lab-Rick-Buglio-Application". The Host Name has to be a unique in Bluemix. Using your First and Last name should make it unique. If you get an error that the name is not unique add your middle initial, if you have one, or use your Bluemix account email address instead.

5. **Select** the "Create" button and the application creation process will begin. 

<img src="./media/Step4-image-04.png" />

> You are taken to the application page and Bluemix will begin starting the application. You will see a starting status with a spinning wheel. Wait until you see that the application is a running status.

6. **Select** the "Dashboard" button in the left side main menu when the application is in a running state. This will take you back to your Bluemix account dashboard.

<img src="./media/Step4-image-05.png" />

> You should see your newly created application in the All Apps section of your Bluemix dashboard.

## Step 5: Create a Watson Analytics Account

You will need a Watson Analytics account. If you **don't** have an account:

### [Click Here to Register for a Watson Analytics account](https://watson.analytics.ibmcloud.com/product)

<img src="./media/Step5-image-01.png" />

1. Click on the “Try it for free” button.

<img src="./media/Step5-image-02.png"/>
   
2.  You will now be prompted to setup an IBM account using the sign-up form as shown above. However, if you already have an IBM account, which you should haveid, one was created for you when you created a Bluemix account, **Select** the "Log in" link to begin creating your Watson Analtics account using the same exact email address you used to create your Bluemix account, this will be your IBM account.

<img src="./media/Step5-image-03.png"/>

5.  To activate your IBMid, you will be sent an email by ibmacct@us.ibm.com with a “Confirmation code” (7 digit number), that you can retrieve from your email box and type it on the sign-up page as shown below.

<img src="./media/Step5-image-05.png"/>

6.  At this point, you will see a status screen saying “Your services are being setup” but within a few seconds your account will be setup and you’ll see a page as below confirming your 30-day trial subscription to “IBM Watson Analytics Professional Single User”!...

<img src="./media/Step5-image-06.png"/>

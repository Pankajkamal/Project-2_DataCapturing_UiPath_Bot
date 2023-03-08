<b> Introduction </b>
This simple bot will be copy-pasting data from an excel spreadsheet into a web and desktop application.

A common daily task of data capturer's life copy-pasting data from excel spreadsheet into a web or desktop application. This bot fully-automates that task. The bot copy-pastes 100 lines of customer data into their respective input fields of web application and desktop application. The bot performs both the web and desktop application data capturing simultaneously. This bot done the job faster than human's and without any error with 100% accuracy.

<b> Technologies </b>

<b> UiPath Studio | RPA Development </b>

<b> Workflow and Activity Details </b>

This bot has three workflows.
1. Main Workflow
2. Web application Data Capturing Workflow
3. Desktop Application Data Capturing Workflow

<b> 1. Main Workflow: </b> This workflow is invoking Web application and Desktop Application workflow for parallel running the bot. <br>
Activity Details of Main Workflow: -<br>
<b> 1. Parallel Activity: </b> This activity is use for running web and desktop application data capturing workflow on simultaneously.<br>
<b> 2. Invoke Activity: </b> This activity is use for invoking web and desktop application data capturing workflow in main workflow.<br>
<b> 3. Log Message Activity: </b> This activity is use for showing a log message after completing the bot. 

<b> 2. Web Application Data Capturing Workflow: </b> This workflow has all activity to capture data from excel spreadsheet into web application(https://www.theautomationchallenge.com/crm).
<br> Activity Details of Web Application Data Capturing Workflow:- <br>
<b> 1. Log Message Activity: </b> This activity is use for showing a log message of starting the bot.<br>
<b> 2. Read Range Workbook Activity: </b> This activity is use for reading the customer data from excel spreadsheet then store data into a data table variable.<br>
<b> 3. Open Browser Activity: </b> This activity is use for opening a chrome browser inside a web application. web application link is https://www.theautomationchallenge.com/crm.<br>
<b> 4. Attach Browser Activity: </b> This activity is use for attaching chrome browser and web application window.<br>
<b> 5. For Each Row Activity: </b> This activity is use for looping through each row of the data table that we created. Which is this customer data.<br>
<b> 6. Type Into Activity: </b> This activity is use for type customer data in web application form fields.<br>
<b> 7. If Activity: </b> This activity is use for Checking the gender from customer data for selecting the gender on web application.<br>
<b> 8. Click Activity: </b> This activity is use for clicking radio check box male and female and click add button.<br>
<b> 9. Select Item: </b> This activity is use for selecting the state Name in select fields.<br>   

<b> 2. Desktop Application Data Capturing Workflow: </b> This workflow has all activity to capture data from excel spreadsheet into Desktop application.<br>
Activity Details of Web Application Data Capturing Workflow:-<br>
<b> 1. Log Message Activity: </b> This activity is use for showing a log message of starting the bot.<br>
<b> 2. Read Range Workbook Activity: </b> This activity is use for reading the customer data from excel spreadsheet then store data into a data table variable.<br>
<b> 3. Open Application Activity: </b> This activity is use for opening a Simple Desktop App application.<br>
<b> 4. Attach Window Activity: </b> This activity is use for attaching Simple Desktop application window.<br>
<b> 5. For Each Row Activity: </b> This activity is use for looping through each row of the data table that we created. Which is this customer data.<br>
<b> 6. Type Into Activity: </b> This activity is use for type customer data in Desktop application form fields.<br>
<b> 7. If Activity: </b> This activity is use for Checking the gender from customer data for selecting the gender on Desktop application.<br>
<b> 8. Click Activity: </b> This activity is use for clicking radio check box male and female and click save button.<br>
<b> 9. Select Item: </b> This activity is use for selecting the state Name in select fields.<br> 

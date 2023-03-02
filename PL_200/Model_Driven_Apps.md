# 2 Canvas Power Apps

## 2.1   Add new environment

Setting> Admin center> click **Environment** on the left hand side> click **+New** on the top > You can configure the new environment:

- Name

- Type: Production, developer, sandbox, trial

  If you choose developer, then a database is automatically created in the environment. 

## 2.2   Create database table 

Powerapps home page > Tables tab on the left> +New> You can add table display name (singular) and primary column name.

**Note:** 

Difference between primary column and primary key in a database table:
Primary key needs to be unique in  a database table, but primary column not. 



After that, go to Tables tab again>selected the created table> click column, add all other columns

## 2.3   Import sample data

### 2.3.1 Import from excel

Go to the created table > Import tab on the top> Import data in excel, you can add data from excel or CSV file in this way. After you upload the sample excel file, you need to do the column mapping. Then save and import data.

## 2.4 Add relationship 

Inside a table, add a relationship to another table. This will add a column, please name column as **XXX Lookup**

## 2.5 Edit in excel

Select the table you want to edit > Edit tab on the top, choose **Edit data in excel** from drop down> Sign in to add add-in to allow to edit in excel, just for the first time > Click enable editing, all the data appear.

After you edit the column, then you need click **publish** to submit the data in PowerApps environment. 

### 2.5.2 How to edit checkup column

The checkup column is the column created when you create a relationship between 2 tables. 

To enter the data for it, you put the mouse to the column, you will see the data from the related table shows up on the right hand side. We need to select the GUID number, not type the actual data, because excel can only recognize GUID. Each GUID is unique. You can not copy paste the GUID, please select it for each column. 

If you type a text on the checkup column, you cannot see any data from the system created checkup column. After edit, you can check the data in the system created checkup column and see if it is correct. 

After publish the update, the actual data in the checkup table is visible, you will not see GUID like in excel. The data type is not text, if you click it, a card is showed up. 

## 2.6 Create canvas app

On the PowerApps home page> select **Create** tab on the left hand side>select from **Dataverse**> click the dataverse, all tables appear> choose the table you wish> click connect, a CRUD canvas app will be created

You can use preview (play) button to test the actual app.

For editing the app, hold on alt key, then click the button or arrow to navigate the page.

## 2.7 App checker

App checker is for canvas app only. 

Solution checker is used for model-driven apps. 


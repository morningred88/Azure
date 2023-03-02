# 3 Model-Driven Apps

## 3.1   Create model-drive app

PowerApps home page> Apps tab> select Model-drive > Give an app name, all others leave default> create app

Then go to setting > choose classic designer

Component is classic designer: 

- Area

- Group: Heading

- Subarea: each page

## 3.2   Add a chart

There are 3 ways to add a chart: 

- From table
- From app designer
- From app: Show chart tab> click 3 dots> click new, to add a chart

## 2.3   Report options

- Chart
- Import Power BI tile
- Create report using RDL

## 2.4 Create RDL report

select the application> click on 3 dots besides the app name> Edit> Add page>Dataverse table >Next>Enter report, select report table> Save and publish

Refresh the application> Go to Reports page> click new> Then click report wizard>Start new report>Give report name> primary record type: table used for report> select view> Next,  lay out Fields, you can add groups or columns from the table>Next, Fromat report, you can choose table, chart or both>Next, report summary > Finish

## 2.4 Add command bar

Each site has a form and a view pages.

Go to the site, select Edit command bar from the site> select where to add> either main grid> next, you can see all the command.

Click new > select command, this will add a button> choose Power Fx langugage> The library will be installed for the first time.

Click new > select drop down, this will add a drop down list

After you save and publish, you will see a button on the top of the page, with the label as NewCommand. Of course, you can change the label in the command editor page. 

### 2.4.1 Command action

#### 2.4.1.1 Notify()

```
Notify("Hello " & Self.Selected.Item.'Pet Owner Name', NotificationType.Information)
```

#### 2.4.1.2 Confirm() and if statement

```
If(Confirm("Do you want to go back to the list?", {Title:"What do you want to do?"}), Navigate('Pet Owners'), Launch("http://www.microsoft.com"))
```


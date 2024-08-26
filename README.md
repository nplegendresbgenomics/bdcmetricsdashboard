# NHLBI BDC Metrics Dashboard
This Repository is for the NHLBI BDC Metrics Dashboard. A proof of Concept of the Dashboard, built in Tableau Public, can be found here: https://public.tableau.com/app/profile/gireesh.subramaniam/viz/PlatformMetricsDashboard/ExecutiveMetricsDashboard

# Developer Guide

## Step 1 - Find your template

We have templates for either search or workspace environments:

* Search Platforms: <https://github.com/gireeshsubrama/bdcmetricsdashboard/blob/main/platformdata/searchplatforms/Search_Platform_Template.csv>
* Analysis Platforms: <https://github.com/gireeshsubrama/bdcmetricsdashboard/blob/main/platformdata/analysisplatforms/Analysis_Platform_Template.csv>

## Step 2 - Generate your data as CSV

Use the templates to generate your data to place in the BDC Metrics AWS Bucket

## Step 3 - Get access to the BDC metrics bucket

* Email Gireesh Subramaniam <gireesh.subramaniam@nih.gov> your AWS credential ID to get access to the bucket
* Please CC Noble Dzakpasu <noble.dzakpasu@nih.gov> as well for NHLBI approval 
* Once given access, please upload metrics CSV files into the folder for your given platform
* bucket is 'nih-nhlbi-bdc-metrics-dashboard': <https://us-east-1.console.aws.amazon.com/s3/buckets/nih-nhlbi-bdc-metrics-dashboard?region=us-east-1&bucketType=general&tab=objects>
* Filepath is Metrics_Upload/<Platform_Name>/<Year>
* Each folder should contain one CSV file, regenerated and overwritten with each refresh.

## Step 4 - Explore data

* The Power BI Dashboard will be available in the GRP-NHLBI-ITAC Power BI Workspace which is managed by NHLBI.

## Metric Field Definitions

### Logins:
* PIC-SURE: Total logins to Authorized PIC-SURE via eRA Commons or BDC Developer Login
* Gen3: Total Logins to Gen3, via NIH login or BDC Developer Login
* Terra: Total Logins to Terra via Google or Microsoft
* Seven Bridges: Total logins to Seven Bridges via eRA Commons or BDC Developer Login

### Search Events:
* Dug: Typing a text string in the search bar and hitting Search
* PIC-SURE: The total number of searches (A text string typed into the search bar and searched) and queries (Using the database filter tools to find a specific set of data)
* Gen3: The number of Explorer Filters used on Gen3’s Exploration page.
* Seven Bridges: The total of:
  1) The number of times the “Explore Selected” button has been clicked on the Data Browser.
  2) The number of filters added in Faceted Search.
  3) The number of times “Explore in Data Browser” has been clicked in the Data Overview page.
  4) The number of searches performed in the Study Variable Explorer.
  5) The number of times “Query dataset” has been clicked in the Annotation Explorer.

### Exports: 
* PIC-SURE: The number of times a cohort has been Exported to Seven Bridges, Exported to Terra, or downloaded as either a CSV or PFB
* Gen3: The number of times a cohort has been exported to CGC, CAVATICA, BDC (Seven Bridges), Terra, or exported as a PFB

### Imports: 
* Terra: The number of times data has been imported into the platform by a user into a Terra Workspace (BYOD Data).
* Seven Bridges: The number of times data has been imported into the platform by a user into a Seven Bridges Project (BYOD Data).

### Workflows Run:
* Terra: The total number of workflows run in a Terra Workspace.
* Seven Bridges: The total number of workflows run in a Seven Bridges Project.

### Notebooks/Interactive Analyses Run:
* Terra: The total number of interactive analyses run in a Terra workspace using JupyterLab, RStudio, Bioconductor or Galaxy.
* Seven Bridges: The total number of interactive Data Studio analysis started using JuypterLab, RStudio, or SAS Studio.





# Examples
<img width="682" alt="Executive Metrics Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/a4f832f9-a7e5-42b7-a05e-1b6c21ab49de">

<img width="679" alt="Search Metrics Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/49518a57-9e0f-42ab-aa7e-5f864e8be9df">

<img width="684" alt="Analysis Metrics Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/d3508050-4de5-4b0f-ba30-4c4576e85c43">

<img width="681" alt="Data Ingest Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/a3a82397-94a5-4238-89b2-9ce1b59d13f4">

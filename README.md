# NHLBI BDC Metrics Dashboard
This Repository is for the NHLBI BDC Metrics Dashboard. A proof of Concept of the Dashboard, built in Tableau Public, can be found here: https://public.tableau.com/app/profile/gireesh.subramaniam/viz/PlatformMetricsDashboard/ExecutiveMetricsDashboard

# Developer Guide

## Step 1 - find your template

We have templates for either search or workspace environments:

* Search Platforms: <https://github.com/gireeshsubrama/bdcmetricsdashboard/blob/main/platformdata/searchplatforms/Search_Platform_Template.csv>
* Analysis Platforms: <https://github.com/gireeshsubrama/bdcmetricsdashboard/blob/main/platformdata/analysisplatforms/Analysis_Platform_Template.csv>

## Step 2 - generate your data as CSV

Use the templates to generate your data to place in the BDC Metrics AWS Bucket

## Step 3 - Get access to the BDC metrics bucket

* email Gireesh Subramaniam <gireesh.subramaniam@nih.gov> your AWS credential ID to get access to the bucket
* Please CC Noble Dzakpasu <noble.dzakpasu@nih.gov> as well for NHLBI approval 
* Once given access, please upload metrics CSV files into the folder for your given platform
* bucket is 'nih-nhlbi-bdc-metrics-dashboard': <https://us-east-1.console.aws.amazon.com/s3/buckets/nih-nhlbi-bdc-metrics-dashboard?region=us-east-1&bucketType=general&tab=objects>
* Filepath is Metrics_Upload/<Platform_Name>/<Year>
* Each folder should contain one CSV file, regenerated and overwritten with each refresh.

## Step 4 - Explore data

* The Power BI Dashboard will be available in the GRP-NHLBI-ITAC Power BI Workspace which is managed by NHLBI.

# Examples
<img width="682" alt="Executive Metrics Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/a4f832f9-a7e5-42b7-a05e-1b6c21ab49de">

<img width="679" alt="Search Metrics Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/49518a57-9e0f-42ab-aa7e-5f864e8be9df">

<img width="684" alt="Analysis Metrics Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/d3508050-4de5-4b0f-ba30-4c4576e85c43">

<img width="681" alt="Data Ingest Dashboard" src="https://github.com/gireeshsubrama/bdcmetricsdashboard/assets/148978711/a3a82397-94a5-4238-89b2-9ce1b59d13f4">

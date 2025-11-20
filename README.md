# DatabaseChex-Onboarding-Template

## Deploy to Azure

Click the button below to deploy this template directly to your Azure subscription:

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAmpedData%2FDatabaseChex-Onboarding-Template%2Fmain%2FARMTemplate%2FAzureLightHouseDelegationTemplate.json
)

## Introduction
Most small IT teams are responsible for helpdesk tickets, user onboarding, cybersecurity, cloud management, budgeting, and keeping critical systems online. Azure SQL adds another layer of responsibility, but most teams don't have the time or specialized database skills to keep it running at its best. Slow performance, failing jobs, and hidden configuration issues can quietly build up until something breaks.

Database Chex solves this by acting like an automated database expert that never sleeps as it monitors your Azure SQL database, detecting issues early, explaining them in plain English, and even fixing many of them automatically.

Database Chex gives small IT teams the visibility, confidence, and peace of mind they've never had before.

## What This Template Is
This template is a simple file that helps Azure know that Database Chex is allowed to view your Azure SQL databases so it can check their health and performance.<br>
It uses a tool called Azure Lighthouse, which is Microsoft's built-in, secure way for one company (like Database Chex) to safely help manage resources in another company's Azure subscription.<br>
Think of it like giving a mechanic permission to look under the hood of your car, but not permission to drive it away, sell it, or change anything without you knowing.

## Why Database Chex Needs This
To do its job, Database Chex needs to:
-	See what databases you have
-	Read performance information (like speed, memory, and errors)
-	Look for problems before they cause slowdowns or downtime
-	Run checks to make sure your databases are healthy
-	Run small automated fixes when something is wrong (Monitor Pro and Monitor Enterprise licenses only)

Without the template, Database Chex has no way to safely access your environment.
With the template, you give Database Chex the **exact, limited** permissions needed and nothing more.

## What You Can Expect
After you deploy this template:
-	Database Chex can access your Azure subscription
-	It finds your Azure SQL databases
-	It begins checking their health
-	It builds your scorecards
-	It starts sending database insights and alerts if anything looks risky
-	It gives you dashboards so you can understand what's going on

All of this happens automatically.<br>
You don't have to set up anything manually.

## The Type of Access This Template Gives
This is very important for customers to understand, so we explain it clearly:
1.	**Reader Access**<br>
    Database Chex can only look at your Azure SQL resources it cannot change anything.  This lets Database Chex read performance metrics, such as CPU, memory, storage, and slow queries.
2.	**Limited Contributor Access** (Monitor Pro and Monitor Enterprise licenses only)<br>
    This allows Database Chex to run optional automations (like fixing a common configuration issue).<br>
    These are tightly restricted and cannot touch anything outside of what the automation specifically needs.

Database Chex cannot delete anything, change anything major, or access unrelated parts of your environment.

## Who Can Deploy the Template
You can only deploy the template if you have the right permissions in your Azure tenant.
Most people who deploy this template fit one of these roles:
-	They are the Azure subscription owner
-	They manage Azure resources for their organization
-	They are responsible for security or infrastructure
-	They are the main IT contact

If you cannot deploy the template, ask your Azure admin to do it for you.

## Before You Begin
Make sure:
1.	You have received an email from Database Chex requesting access to your Azure tenant.
2.	You are logged in to the Azure Portal.
3.	You know which subscription you want Database Chex to monitor.
4.	You have permission to add a service provider in Azure.

If you are missing any of these, you will not be able to deploy the template successfully.

## How to Deploy the Template 
1.	Click the "Deploy to Azure" button that Database Chex provides.
2.	Azure will open a page showing the template details.
3.	Choose the correct subscription.
4.	Review the settings (everything is pre-filled for you).
5.	Click "Review + Create".
6.	Click "Create".

Azure processes the template and sets up the connection.<br>
This usually takes **1 hour**.<br>
When it's done, Database Chex immediately begins identifying database in your environment your environment.

## What Happens Next
1. **Subscription Detection**<br>
    Database Chex sees the subscription you connected.
2. **Database Discovery**<br>
    It looks for Azure SQL Databases
3. **Assign Database Chex Licenses**<br>
    After Database Chex has identified all the databases that can be monitored in your subscription, you will need to assign a Database Chex license to each database that you are wanting to monitor.
4. **Health Scanning**<br>
    It checks dozens of database performance metrics such as:
    -	Slow performance
    -	Deadlocks
    -	Storage issues
    -	Missing indexes
    -	Long-running queries
5. **Scorecard Creation**<br>
    Database Chex assigns each database a simple:
    -	**Green** (healthy)
    -	**Yellow** (warning)
    -	**Red** (needs attention)
    
    This becomes your "Traffic-Light Scorecard".
6. **Dashboards + Insights**<br>
    Your Database Chex dashboard begins filling with insights and recommendations.
7. **Alerts & Notifications**<br>
    If something looks serious, Database Chex sends alerts in plain English to you.
8. **Automated Fixes**<br>
    If you are using Monitor Pro licenses, Database Chex may run safe automated fixes.

## Removing Access
You can remove Database Chex access anytime.<br>
There is no lock-in.<br>
Just go to the Azure Portal, search for "Service Providers", find "Database Chex", and remove it.<br>
Once you do this, Database Chex instantly loses access.

## Support
If you need help at any point:
Email: support@databasechex.com
Website: databasechex.com
We're happy to walk you through deployment or troubleshoot any issues.
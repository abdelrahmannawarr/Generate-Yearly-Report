# Generate Yearly Report – UiPath Project

## Overview
This UiPath project automates the process of downloading monthly reports from a web portal, consolidating them into a single yearly Excel report, and emailing the final report to stakeholders. It reduces manual effort and ensures accuracy in reporting.

## Objective
- Log in to a web portal and navigate to the reports section
- Download all monthly reports for a given year
- Merge and filter data into a single structured Excel file
- Email the final report automatically to specified recipients

## Technologies Used
- UiPath Studio
- Excel Activities
- Web Automation (Click, Type Into, Attach Browser, etc.)
- File and Folder Activities
- SMTP / Outlook Email Activities
- Dynamic Selectors
- Exception Handling

## Features
- Downloads monthly reports dynamically based on selected year
- Merges multiple Excel files into one
- Filters and formats data as needed
- Sends final yearly report as an email attachment
- Logs key steps and handles common errors

## Prerequisites
- UiPath Studio installed
- Access to the target web portal
- Email account configured (SMTP or Outlook)
- Monthly reports available for download
- Year input (can be hardcoded or from config)

## How It Works
1. Bot navigates to the web portal and logs in.
2. Loops through each month to download reports.
3. Stores all files in a temporary folder.
4. Reads and filters data from each file.
5. Merges them into one final Excel file.
6. Sends the final report via email.
7. Cleans up temporary files.

## Output
- Final merged Excel file (e.g., `YearlyReport_2024.xlsx`)
- Email sent with report as an attachment
- Execution logs stored locally (if enabled)

## How to Use
1. Update the Config file with web URLs, email settings, and folders.
2. Run the process from UiPath Studio or Orchestrator.
3. Monitor email output and generated report.

## Author
Created as part of an RPA training project to demonstrate end-to-end automation involving file handling, web interaction, Excel operations, and email automation.

---

You can enhance the project by adding user prompts for year selection, report validation, or integrating with a database for storage.

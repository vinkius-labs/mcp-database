# Watershed Climate MCP Server

Automate carbon measurement and reporting via Watershed — manage inventories, upload emissions data, and track reduction targets directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/watershed-climate)

## Overview
**Category:** the-unthinkable
**Tools Count:** 16

## Description
Connect your **Watershed Climate** organization to any AI agent and take full control of your carbon measurement, reporting, and reduction workflows through natural conversation.

### What you can do

- **Data Uploads** — Create upload containers, add activity data records (electricity, travel, shipping), and validate data quality
- **Batch Data Ingestion** — Upload multiple activity records in batch with proper formatting and emission factor mapping
- **GHG Inventories** — List and inspect greenhouse gas inventories with Scope 1, 2, and 3 emissions breakdowns
- **Emissions Measurements** — Query calculated carbon footprint measurements filtered by inventory or year
- **Processing Tasks** — Monitor async processing tasks from upload submissions with real-time status checks
- **Reports & Disclosures** — List and access generated sustainability reports (CDP, TCFD, custom formats)
- **Reduction Targets** — View configured emissions reduction targets aligned with SBTi and net-zero commitments

### How it works

1. Subscribe to this server
2. Enter your Watershed API Key from dashboard.watershedclimate.com
3. Start managing your climate program from Claude, Cursor, or any MCP-compatible client

No more manual CSV uploads or navigating complex dashboards. Your AI acts as a dedicated sustainability analyst or carbon accounting specialist.

### Who is this for?

- **Sustainability Teams** — instantly upload activity data, validate uploads, and check inventory results without opening the Watershed dashboard
- **ESG Analysts** — query emissions measurements and reduction targets directly to generate carbon footprint insights
- **Operations & Supply Chain** — automate batch data ingestion for electricity, travel, and logistics emissions tracking
- **Climate Leads** — monitor processing tasks and report generation status across multiple organizational inventories


## Available Tools
- **create_upload**: An upload is required before you can add data records to Watershed.
After creating an upload, you add data records to it, validate the data, and then submit it for processing.
The upload acts as a batch grouping mechanism for related activity data.
You can optionally provide a name and description to identify the upload purpose.

Create a new data upload container in Watershed
- **delete_upload_data_record**: Use this to remove 
incorrect or unwanted data before validating and submitting the upload.
This action cannot be undone. The record_id is obtained from list_upload_data_records.

Delete a specific data record from an upload
- **get_inventory**: Use the inventory_id from list_inventories to inspect detailed carbon footprint results
and understand your organization's emissions composition.

Get detailed information about a specific GHG inventory
- **get_report**: Use the report_id from list_reports to access the full report details including
generated files, disclosure frameworks covered, and emissions data summarized.
Reports are typically generated after inventories are complete and validated.

Get detailed information about a specific report
- **get_task_status**: When you submit an upload for processing, a task is created and returns a task_id.
Use this tool to check if the processing is complete, still in progress, or failed.
Task status is useful for monitoring large data submissions that may take time to process.

Check status of a processing task (e.g., upload submission)
- **get_upload**: Use the upload_id from list_uploads to inspect details 
before adding data or submitting for validation.

Get details of a specific data upload
- **list_inventories**: An inventory represents your organization's carbon footprint measurement for a specific year,
containing Scope 1 (direct), Scope 2 (energy), and Scope 3 (value chain) emissions data.
Each inventory has a year, status, and total emissions calculated from submitted activity data.

List all GHG inventories in your Watershed organization
- **list_measurements**: Measurements represent the actual carbon footprint values derived from your uploaded activity data.
You can filter by inventory_id to see measurements for a specific year's inventory,
or by year to see measurements across all inventories for that year.
Each measurement includes the activity type, emission factor used, and calculated CO2e value.

List emissions measurements with optional filters
- **list_reduction_targets**: Reduction targets define your organization's goals for decreasing emissions over time,
often aligned with Science Based Targets initiative (SBTi) or net-zero commitments.
Each target includes baseline year, target year, reduction percentage, and progress tracking.

List all emissions reduction targets configured in your organization
- **list_reports**: Reports are formatted outputs of your climate data for disclosure, analysis, or internal review.
Reports can include CDP disclosures, TCFD reports, or custom carbon footprint summaries.
Each report has metadata about its type, generation date, and scope.

List all available reports in your Watershed organization
- **list_upload_data_records**: Each record contains the activity data that will be processed into emissions measurements.
Use this to review the data before validating and submitting the upload.

List all data records in a specific upload
- **list_uploads**: Uploads are containers for activity data that will be validated and processed into emissions measurements.
Each upload can contain multiple data records representing activities like electricity usage, flights, or shipping.
Use this to see all existing uploads and their IDs before adding data or submitting for processing.

List all data uploads in your Watershed organization
- **submit_upload**: This triggers Watershed's calculation 
engine to convert activity data into emissions measurements using appropriate emission factors.
The upload must be validated successfully before submission. 
The response includes a task_id that can be used to track processing status via get_task_status.
Processing may take some time depending on data volume.

Submit a validated upload for emissions processing
- **update_upload_data_record**: Use this to correct errors 
or modify activity data before validation and submission.
The record_id is obtained from list_upload_data_records. The body should contain the complete 
updated record object with all required fields.

Update a specific data record in an upload
- **upload_data_records**: Each record represents an activity 
that generates emissions (e.g., electricity consumption, business travel, shipping).
Records should follow Watershed's data format with fields like: activity_type, quantity, unit, 
start_date, end_date, location, etc.
You can upload a single record or multiple records in a batch by providing an array of objects.
Example record: { "activity_type": "electricity", "quantity": 1500, "unit": "kWh", "start_date": "2024-01-01", "end_date": "2024-01-31" }

Upload activity data records to an existing upload container
- **validate_upload**: Validation ensures data quality and prevents rejection during the submission phase.
The response includes validation results with any errors or warnings that need to be addressed.
Always validate before submitting to ensure successful processing.

Validate data in an upload before submission


## Installation & Usage

To install and use the **Watershed Climate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/watershed-climate](https://vinkius.com/mcp/watershed-climate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

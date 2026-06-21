# Watershed Climate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/watershed-climate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Automate carbon measurement and reporting via Watershed — manage inventories, upload emissions data, and track reduction targets directly from any AI agent.

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


## Available Tools (16)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Watershed Climate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our GHG inventories and show me the total emissions for 2024."

**🤖 AI Agent:**
> I've found your GHG inventories. You have 2 inventories: 'FY2024 Global Operations' (Inventory ID: inv_2024_global) with total emissions of 12,450 tCO2e (Scope 1: 2,100, Scope 2: 3,850, Scope 3: 6,500) and 'FY2023 Global Operations' with 14,200 tCO2e. Your 2024 footprint shows a 12.3% reduction from 2023. Would you like a detailed breakdown by scope or emission source?

---

**👤 You:**
> "Create a new upload called 'Q1 2024 Electricity Data', add these 3 records: electricity usage for NYC office (50,000 kWh), London office (35,000 kWh), and São Paulo office (28,000 kWh) for January 2024, then validate and submit it."

**🤖 AI Agent:**
> I've completed the full data upload workflow:
1. Created upload 'Q1 2024 Electricity Data' (Upload ID: upl_q1_2024_elec)
2. Added 3 electricity records (NYC: 50,000 kWh, London: 35,000 kWh, São Paulo: 28,000 kWh)
3. Validated the upload — all records passed validation with no errors
4. Submitted for processing (Task ID: task_abc123)

The task is currently processing. I can monitor the status for you. Would you like me to check the task status in a moment?

---

**👤 You:**
> "Show me our reduction targets and current progress toward our net-zero goal."

**🤖 AI Agent:**
> Here are your organization's reduction targets:

1. **SBTi 2030 Target** — Reduce absolute Scope 1+2 emissions by 50% by 2030 (baseline: 2019). Current progress: 28% reduction achieved.
2. **Net-Zero 2040 Target** — Achieve net-zero across all scopes by 2040. Current progress: 35% reduction from 2019 baseline.
3. **Scope 3 Target** — Reduce Scope 3 emissions intensity by 30% per unit of revenue by 2030. Current progress: 18% reduction.

You're on track for the 2030 SBTi target at current reduction rate. Would you like a detailed emissions trend analysis?


## ❓ FAQ

**Q: What is the workflow to upload activity data and get emissions calculated in Watershed?**
The complete workflow is: (1) Use `create_upload` to create an upload container, (2) Use `upload_data_records` to add your activity data records (electricity, flights, shipping, etc.), (3) Use `validate_upload` to check data quality and fix any errors, (4) Use `submit_upload` to send data for emissions calculation, (5) Use `get_task_status` with the returned task_id to monitor processing. Once complete, your measurements appear in the inventory.

**Q: Can I check my organization's total carbon footprint for a specific year?**
Yes! Use `list_inventories` to find your organization's GHG inventories by year. Then use `get_inventory` with the specific inventory_id to see the complete emissions breakdown by Scope 1 (direct), Scope 2 (energy), and Scope 3 (value chain). You can also use `list_measurements` with the year filter to see individual measurement details across all inventories.

**Q: Where do I find my Watershed API key and how do I generate one?**
Log in to your Watershed dashboard at dashboard.watershedclimate.com, navigate to **Organization Settings** in the left menu, then go to the **API** section. Click to generate a new API key. Copy and save this key immediately — it won't be shown again. The key typically starts with `wh_`. Keep it secure as it provides full access to your organization's climate data.

**Q: What types of activity data can I upload to Watershed?**
Watershed accepts a wide range of activity data including: electricity and energy consumption (kWh, therms), business travel (flights, hotels, rental cars), employee commuting, freight and shipping (ton-miles, kg-km), waste generated, water usage, and purchased goods/services. Each record needs fields like activity_type, quantity, unit, start_date, end_date, and optionally location and spend_amount for accurate emissions calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/watershed-climate](https://vinkius.com/mcp/watershed-climate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Watershed Climate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `watershed-climate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Watershed Climate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "watershed-climate": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

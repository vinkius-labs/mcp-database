# TaxBandits MCP Server

File US tax forms electronically including W-2, 1099, and ACA forms with IRS-authorized e-filing and instant status tracking.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/taxbandits)

## Overview
**Category:** erp-operations
**Tools Count:** 6

## Description
Connect your **TaxBandits** account to any AI agent and simplify how you manage tax filings, business records, and IRS submissions through natural conversation.

### What you can do

- **Business Management** — List all registered business entities and create new profiles for tax reporting purposes.
- **Tax Filing Oversight** — List and query filed or draft tax forms (e.g., 1099, W-2, 94x) across multiple tax years.
- **Submission Tracking** — Check the real-time status of your form submissions to ensure successful IRS or state delivery.
- **Transmission Monitoring** — List and inspect form transmissions to keep a record of your filing history.
- **Metadata Retrieval** — Fetch detailed metadata for specific businesses to verify identifiers like EIN and business addresses.
- **Compliance Automation** — Manage your tax reporting lifecycle directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your TaxBandits Client ID and Client Secret (found in your developer portal)
3. Start managing your tax compliance from your favorite AI assistant

### Who is this for?

- **Accountants & CPAs** — quickly retrieve filing statuses and verify business metadata via simple AI commands.
- **Business Owners** — monitor the status of recurring tax forms and ensure compliance directly from the workspace.
- **Tax Software Developers** — test form creation and verify transmission logs via the AI assistant.


## Available Tools
- **create_business**: Pass data as a JSON string.

Create a new business entity
- **get_business_details**: Get specific business details
- **get_submission_status**: Check status of a form submission
- **list_businesses**: List all registered businesses
- **list_tax_forms**: Pass filters as a JSON string.

List tax forms (e.g. 1099)
- **list_transmissions**: List form transmissions


## Installation & Usage

To install and use the **TaxBandits** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taxbandits](https://vinkius.com/mcp/taxbandits)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

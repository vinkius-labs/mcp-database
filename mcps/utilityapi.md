# UtilityAPI MCP Server

Access utility billing, usage data, and meter info from PG&E and 100+ US utilities via a single API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/utilityapi)

## Overview
**Category:** data-management
**Tools Count:** 12

## Description
Connect **UtilityAPI** to any AI agent and access utility billing history, granular usage intervals, and meter data from over 100 US utility companies — including PG&E, Southern California Edison, Con Edison, National Grid, and more — through a single unified API.

### What you can do

- **Supported Utilities** — List all 100+ utility companies available through the platform with their codes and data types
- **Customer Authorizations** — Create and manage authorization forms for customers to securely share their utility data
- **Meter Management** — List all authorized utility meters (service points) with addresses, fuel types, and collection status
- **Billing History** — Retrieve complete billing history with costs, usage amounts (kWh/therms), and billing periods
- **Usage Intervals** — Access granular smart meter interval data (15-min or hourly readings) for detailed energy analysis
- **Historical Collection** — Activate backfilling of historical utility data for newly authorized meters
- **Combined Meter Data** — Get both bills and intervals in a single call for comprehensive energy analysis
- **Event Monitoring** — Monitor webhook events for authorization flows, data collection status, and errors
- **Demo Testing** — Test authorization forms with simulated residential and commercial scenarios before production
- **Billing Summaries** — Track API usage costs and billing periods for your UtilityAPI account

### How it works

1. Subscribe to this server
2. Enter your UtilityAPI API Token
3. Start accessing utility billing and usage data from Claude, Cursor, or any MCP-compatible client

UtilityAPI eliminates the need to integrate with each utility company individually — one API connects to 100+ providers.

### Who is this for?

- **Energy Consultants** — analyze customer utility bills and usage patterns to recommend efficiency improvements and cost savings
- **Solar Installers** — access historical electricity usage to size solar systems accurately and calculate ROI for proposals
- **FinTech & Lending** — verify utility payment history and spending patterns for energy efficiency loan qualification
- **Property Managers** — monitor utility costs across portfolios and identify anomalies in billing or consumption


## Available Tools
- **activate_historical_collection**: Send an array of meter_uids (from list_meters) to begin backfilling historical data. Once activated, the system will start collecting all available historical data for those meters. Use this after a new customer authorization to ensure you get their complete usage history, not just future data. Data collection may take time depending on the utility and data availability.

Activate historical data collection for specific utility meters
- **create_auth_form**: Returns a form_uid that can be used to redirect customers to the authorization flow. The utilityCode parameter must be a valid utility code (from list_utilities). Optional scenario parameter controls the test mode: "residential" (home customer), "commercial" (business customer), or other utility-specific scenarios. Use this to set up new data sharing agreements with utility customers.

Create a new authorization form for customers to share their utility data
- **get_billing_summaries**: Includes billing periods, costs, and meter counts for your UtilityAPI subscription. Optional meterId parameter retrieves summary for a specific meter. Use this to track API usage costs and understand billing periods for your UtilityAPI account.

Get billing account summaries for UtilityAPI accounting
- **get_bills**: Returns utility bills with: start/end dates, total cost (in dollars), energy usage (kWh for electric, therms for gas), utility name, and meter association. The meters parameter is required — provide a single meter UID or comma-separated multiple UIDs. Use this to analyze customer spending on utilities, identify high-cost periods, or provide billing insights. Bills are only available for meters that have been authorized and are actively collecting data.

Get utility billing history for authorized meters
- **get_events**: Events include: new authorization created, meter data available, collection completed, errors, etc. Use this to monitor the status of data collection workflows, debug authorization issues, or build real-time notifications for when customer data becomes available.

Get webhook events from UtilityAPI (authorizations, data collection status)
- **get_form_templates**: Templates define what information is collected during the customer authorization process. Use this to understand available form configurations before creating custom authorization forms. Each template has a unique ID used when creating new forms.

Get authorization form templates used for customer data sharing
- **get_intervals**: This is granular consumption data showing energy usage over time intervals (typically 15-minute or hourly readings from smart meters). Each interval includes: start/end timestamp, usage value (kWh or therms), and cost information. The meters parameter is required — provide meter UID(s). Use this for detailed energy analysis, identifying peak usage patterns, demand response analysis, or building energy models. This is more granular than bills — ideal for time-series analysis.

Get detailed usage interval data (hourly/15-min) for authorized meters
- **get_meter_data**: This is a convenience tool that combines results from get_bills and get_intervals for one meter. Returns: complete bill history (dates, costs, usage) plus granular interval data (time-series readings). Use this when you need a complete picture of a customer's utility data — both the financial (billing) and technical (usage patterns) aspects — for comprehensive energy analysis. The meterUid must be a valid meter UID from list_meters.

Get combined billing and interval data for a specific meter in one call
- **list_authorizations**: Each authorization represents a customer who has granted access to their utility data. Optional referrals parameter filters by a specific referral code (from test submissions). Set includeMeters=true to also return associated meter data with each authorization. Use this to track which customers have authorized data access and get their referral codes for meter queries.

List all customer data sharing authorizations
- **list_meters**: Each meter represents a specific utility service connection (electricity or gas) at a customer location. Meter data includes: utility name, service address, fuel type (electric/gas), collection status, and the unique meter_uid used for fetching bills and intervals. Optional authorizationId filters meters to a specific customer authorization. Use the meter_uid with get_bills and get_intervals to retrieve usage data.

List all authorized utility meters (service points)
- **list_utilities**: Each utility includes its name, utility code (used for form submissions), and supported data types. Use this to find the correct utility code when creating authorization forms or querying utility-specific data. Common utilities include: PG&E (Pacific Gas & Electric), SCE (Southern California Edison), Con Edison, National Grid, and many others across the US.

List all supported utility companies available through UtilityAPI
- **test_form_submission**: Returns a referral_code that can be used to retrieve the test authorization and associated meter data. Use this during development and testing to verify form configurations work correctly before deploying to production. The formId is the uid returned by create_auth_form. The referral_code returned can be used with list_authorizations to retrieve test data.

Test an authorization form to simulate customer authorization and get a referral code


## Installation & Usage

To install and use the **UtilityAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/utilityapi](https://vinkius.com/mcp/utilityapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

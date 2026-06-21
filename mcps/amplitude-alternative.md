# Amplitude MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplitude-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amplitude-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amplitude-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track user behavior, analyze product metrics, and manage cohorts directly from your AI agent using Amplitude's powerful analytics suite.

## Description
Connect your **Amplitude** analytics account to any AI agent to ingest events, query user profiles, and analyze product performance through natural conversation.

### What you can do

- **Event Ingestion** — Send single or high-volume batch events to the Amplitude cloud using `send_events` and `send_batch_events`.
- **User Insights** — Fetch real-time user profiles, recommendations, and cohort memberships with `get_user_profile`.
- **Data Analysis** — Query segmentation metrics for specific events or export raw event data for deep analysis using `get_segmentation` and `export_data`.
- **Cohort Management** — List all behavioral cohorts or create new ones by uploading static lists of IDs with `list_cohorts` and `upload_cohort`.
- **Taxonomy & Governance** — Manage event categories, properties, and audit logs to keep your data clean and secure.

### How it works

1. Subscribe to this server
2. Enter your Amplitude API Key and Secret Key
3. Start analyzing user behavior from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — instantly retrieve event counts, check user properties, and monitor feature adoption without leaving your chat.
- **Data Analysts** — export raw data for specific time ranges and verify event taxonomy on the fly.
- **Growth Engineers** — identify users, manage cohorts, and check experiment variants directly from your development environment.


## Available Tools
- **create_annotation**: Annotate charts with important dates
- **create_category**: Create a new event category (Taxonomy)
- **create_release**: Create a release to track feature impact
- **delete_users**: Submit data deletion requests (GDPR/CCPA)
- **export_data**: Export raw event data in JSON format
- **get_audit_logs**: Export administrative activity logs
- **get_experiment_variant**: Retrieve variant assignments for users (Experiment API)
- **get_segmentation**: Query metrics displayed in Amplitude charts
- **get_user_profile**: Fetch real-time user data and properties
- **group_identify**: Set or update properties for specific groups
- **identify_user**: Update user properties without sending an event
- **list_categories**: Get all event categories (Taxonomy)
- **list_cohorts**: Get all behavioral cohorts
- **list_event_properties**: Get all event properties (Taxonomy)
- **list_event_types**: Get all event types (Taxonomy)
- **list_user_properties**: Get all user properties (Taxonomy)
- **map_user**: Map one user ID to another (Global User ID)
- **send_attribution**: Send attribution data from partners
- **send_batch_events**: Send high-volume data to Amplitude (Batch API)
- **send_events**: Requires an array of event objects.

Send data directly to Amplitude (HTTP V2 API)
- **upload_cohort**: Create a cohort from a list of IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplitude** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Export raw event data from 2023100100 to 2023100123."

**🤖 AI Agent:**
> I've initiated the data export for that range. The raw event data is being retrieved from Amplitude's servers now.

---

**👤 You:**
> "Get the profile and cohort memberships for user ID 'user_123'."

**🤖 AI Agent:**
> Fetching profile for 'user_123'... This user is part of 3 cohorts: 'Power Users', 'Early Adopters', and 'Beta Testers'. Their last active property was 'premium_plan: true'.

---

**👤 You:**
> "List all behavioral cohorts in this project."

**🤖 AI Agent:**
> I found 12 behavioral cohorts. Some notable ones include 'Dormant Users' (ID: 5a2b), 'Weekly Actives' (ID: 9f1c), and 'New Signups' (ID: 3e4d).


## Installation & Usage

To install and use the **Amplitude** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplitude-alternative](https://vinkius.com/mcp/amplitude-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# FDA (openFDA) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fda-openfda)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fda-openfda-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fda-openfda-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access public health data via openFDA — search drug labeling, monitor adverse events, and track food recalls directly through your AI agent.

## Description
Connect to the **openFDA** public database through any AI agent and gain instant access to thousands of datasets regarding drugs, food, and medical devices.

### What you can do

- **Drug Intelligence** — Search official FDA drug labels, NDC directories, and monitor real-time drug shortages flawlessly
- **Safety Monitoring** — Query adverse event reports for drugs, foods, and medical devices to analyze public health trends natively
- **Compliance Tracking** — List recall enforcement reports to stay informed about hazardous food or drug products in circulation
- **Regulatory Insights** — Access Drugs@FDA metadata including approvals, therapeutic equivalents, and manufacturer details
- **Medical Device Data** — Search device classifications and enforcement actions to verify product safety synchronously
- **Public Data Access** — Retrieve raw structured data from the official U.S. Food and Drug Administration API without complex manual exports

### How it works

1. Subscribe to this server
2. Enter your optional openFDA API Key (Settings > API Key at open.fda.gov)
3. Start querying public health data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Professionals** — quickly look up drug labels or side effect profiles during research or consultation
- **Compliance Officers** — monitor food and drug recall reports across specific regions or manufacturers
- **Data Researchers** — pull aggregated public health metrics directly into your AI-powered analysis workflow


## Available Tools
- **get_drug_shortages**: Get current and resolved drug shortages
- **get_usage**: Get current API usage and rate limit info
- **search_device_adverse_events**: Search for adverse event reports for medical devices
- **search_device_classification**: Search for medical device classifications
- **search_device_enforcement**: Search for medical device recall enforcement reports
- **search_drug_adverse_events**: Search for adverse event reports for drugs
- **search_drug_approvals**: Search for FDA-approved brand name and generic drugs
- **search_drug_enforcement**: Search for drug recall enforcement reports
- **search_drug_labels**: Search for FDA drug product labeling
- **search_food_adverse_events**: Search for adverse event reports for foods
- **search_food_enforcement**: Search for food recall enforcement reports
- **search_ndc**: Search the National Drug Code directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FDA (openFDA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for adverse events reported for Ibuprofen."

**🤖 AI Agent:**
> Searching drug adverse events... I've retrieved the latest reports. Common reported reactions include nausea and headache. Would you like to see the demographic breakdown of these reports?

---

**👤 You:**
> "Are there any recent food recalls in New York?"

**🤖 AI Agent:**
> Inspecting food enforcement reports... I found 3 recent recalls affecting New York, including a voluntary recall of organic spinach due to potential contamination. Shall I list the specific product details?

---

**👤 You:**
> "Show me the label information for Advil."

**🤖 AI Agent:**
> Retrieving Advil product label... I've found the official FDA labeling. It contains detailed indications, dosage instructions, and warnings. Would you like me to summarize the usage guidelines?


## Installation & Usage

To install and use the **FDA (openFDA)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fda-openfda](https://vinkius.com/mcp/fda-openfda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

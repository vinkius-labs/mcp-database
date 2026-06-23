# Redox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/redox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect to the Redox healthcare API to search patients, retrieve clinical conditions, and write back observations directly from your AI agent.

## Description
Integrate your **Redox** environment with any AI agent to streamline healthcare interoperability. This server allows you to interact with clinical data using both FHIR standards and Redox Data Models through natural language.

### What you can do

- **Patient Discovery** — Search for patient records across connected healthcare systems using specific identifiers and destination slugs.
- **Clinical Insights** — Retrieve active diagnoses and conditions (problem lists) for specific patients to provide medical context.
- **Clinical Writeback** — Save vitals and clinical observations back to the EHR by sending structured FHIR bundles.
- **Data Model Events** — Send asynchronous notifications or synchronous queries using standardized Redox JSON Data Models for broad interoperability.
- **Environment Management** — Seamlessly switch between development and production environments for testing and deployment.

### How it works

1. Subscribe to this server
2. Enter your Redox API Key
3. Start querying patient data or posting clinical observations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HealthTech Developers** — Test clinical integrations and verify FHIR resource mapping directly from your coding environment.
- **Clinical Operations** — Quickly look up patient conditions or identifiers without navigating complex EHR interfaces.
- **Digital Health Startups** — Accelerate the development of AI-driven medical assistants by providing them with real-time access to clinical data.


## Available Tools (4)
- **create_observation**: Save vitals or observations (Writeback)
- **post_data_model**: Send a Redox Data Model API event
- **search_condition**: g., problem-list-item) associated with a specific patient ID.

Retrieve diagnoses/conditions for a patient
- **search_patient**: Search for a patient in Redox FHIR API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Redox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for patient identifier 'urn:redox:source:MR|12345' in the production environment for destination 'clinical-hub'."

**🤖 AI Agent:**
> I've initiated the search in the clinical-hub destination. I found a patient record matching that identifier. Would you like to see the full FHIR resource details?

---

**👤 You:**
> "Retrieve all active conditions for patient ID 'P123' in the development environment."

**🤖 AI Agent:**
> I've fetched the conditions for patient P123. The list includes 'Essential hypertension' and 'Type 2 diabetes mellitus'. Do you need the specific codes or onset dates for these?

---

**👤 You:**
> "Post a Redox Data Model event for a new appointment notification using this JSON payload."

**🤖 AI Agent:**
> I've sent the Data Model payload to the Redox API. The event has been successfully queued for processing. Here is the response metadata from the server.


## ❓ FAQ

**Q: Can I search for patients across different healthcare systems?**
Yes, by using the `search_patient` tool with the specific `destination_slug` and `identifier`, you can query any connected system in your Redox network.

**Q: Does this support writing clinical data back to an EHR?**
Yes. The `create_observation` tool allows you to perform writeback operations by sending FHIR bundles containing vitals or other clinical observations.

**Q: What is the difference between FHIR tools and the Data Model tool?**
The `search_patient` and `search_condition` tools use the FHIR API for standardized resource access, while `post_data_model` uses Redox's proprietary JSON Data Models for broader interoperability events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redox](https://vinkius.com/mcp/redox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Redox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `redox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Redox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "redox": {
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

# Factored Quality MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/factored-quality)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage quality control via Factored Quality — track inspections, audits, and lab tests directly through your AI agent.

## Description
Connect your **Factored Quality** account to any AI agent and take full control of your quality control (QC), audit, and compliance data through natural conversation.

### What you can do

- **Inspection Tracking** — List all quality control inspections and fetch detailed results for any batch
- **Factory Audits** — Inspect audit reports and compliance data for your manufacturing partners
- **Lab Testing** — Access and monitor the status and results of your product lab tests
- **Booking Management** — Create and manage bookings for QC services directly from the cloud
- **Supplier Visibility** — Query details about your suppliers and their quality performance history
- **Real-time Data** — Extract raw QC data to power your supply chain analytics and decision-making

### How it works

1. Subscribe to this server
2. Enter your Factored Quality API Key
3. Start managing your quality control from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor inspection results and green-light goods for pickup without leaving your workflow
- **Quality Engineers** — review lab test data and audit reports through simple natural language queries
- **Supply Chain Leaders** — track supplier performance and compliance status across your global network


## Available Tools (12)
- **create_booking**: Book a new quality control service
- **get_audit**: Get details for a specific audit
- **get_booking**: Get details for a specific booking
- **get_inspection**: Get details for a specific inspection
- **get_lab_test**: Get details for a specific lab test
- **get_me**: Get current API user profile info
- **get_supplier**: Get details for a specific supplier
- **list_audits**: List all factory audits
- **list_bookings**: List all QC service bookings
- **list_inspections**: List all quality control inspections
- **list_lab_tests**: List all lab tests
- **list_suppliers**: List all suppliers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Factored Quality** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent quality control inspections."

**🤖 AI Agent:**
> I've retrieved your recent inspections. You have 5 inspections in progress and 12 completed this month. The latest one for 'Summer SKU-101' at Factory X passed with a score of 98%.

---

**👤 You:**
> "Show me the status of the latest lab test for product Y."

**🤖 AI Agent:**
> Fetching lab test results... The latest test for 'Product Y' (ID: 789) is COMPLETED. The results show all materials comply with REACH and RoHS standards.

---

**👤 You:**
> "Book a new inspection for Supplier Z next week."

**🤖 AI Agent:**
> Booking started... I've initiated a new inspection request for 'Supplier Z'. Please provide the specific PO number and SKU details to finalize the booking.


## ❓ FAQ

**Q: How do I obtain my Factored Quality API Key?**
Users with Company Admin access can generate API keys by navigating to **Settings > API Keys** in the Factored Quality Portal.

**Q: Can I integrate this with my logistics provider?**
Yes, you can use the API data to automate workflows with freight forwarders, such as green-lighting goods for pickup based on passing inspection results.

**Q: Is it possible to view full lab test reports?**
The `get_lab_test` tool retrieves detailed metadata and results for your lab tests. For full PDF reports, you can find the direct link in the metadata returned by the API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/factored-quality](https://vinkius.com/mcp/factored-quality)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Factored Quality** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `factored-quality` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Factored Quality** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "factored-quality": {
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

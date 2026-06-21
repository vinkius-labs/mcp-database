# DOD Contracts (FPDS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dod-contracts-fpds)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search and analyze Department of Defense (DOD) and federal contracts via the FPDS Atom Feed directly from your AI agent.

## Description
Connect your AI agent to the **Federal Procurement Data System (FPDS)** to monitor government spending and analyze contract awards in real-time.

### What you can do

- **Contract Search** — Query the massive database of federal procurement actions using standard FPDS search syntax.
- **DOD Targeting** — Specifically isolate Department of Defense data by filtering for Department ID '9700' or Agency Code '9700'.
- **Market Intelligence** — Track vendor performance, identify upcoming procurement trends, and analyze historical spending patterns.
- **Pagination Support** — Navigate through large result sets using the start parameter to fetch data in batches of 10.

### How it works

1. Subscribe to this server
2. Configure your access identifier
3. Start querying federal contracts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Government Contractors** — monitor competitors and find new opportunities within the DOD.
- **Data Analysts** — extract raw XML contract data for spending analysis and reporting.
- **Journalists & Researchers** — track government transparency and public spending across federal agencies.


## Available Tools
- **search_contracts**: To target DOD contracts, include DEPARTMENT_ID:"9700" or AGENCY_CODE:"9700" in the sQuery parameter. Returns XML data containing contract entries.

Search federal contracts via FPDS Atom Feed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DOD Contracts (FPDS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for DOD contracts related to 'cybersecurity' using search_contracts."

**🤖 AI Agent:**
> I've searched the FPDS for DOD cybersecurity contracts. I found several entries, including a recent award for 'Network Defense Services' to CyberCorp and a 'Security Operations' contract for the Air Force. Would you like details on a specific entry?

---

**👤 You:**
> "Find federal contracts for 'Lockheed Martin' using search_contracts."

**🤖 AI Agent:**
> Querying FPDS for 'Lockheed Martin'... I've retrieved the latest 10 contract actions. They include various aerospace and defense projects across different agencies. Should I list the PIIDs and award amounts for these?

---

**👤 You:**
> "Get the next 10 results for the DOD 'cloud services' search using search_contracts with start=10."

**🤖 AI Agent:**
> Fetching the next page of results (records 11-20) for DOD cloud services... I've found additional contracts involving cloud migration and infrastructure support. Would you like me to summarize the vendors involved in this batch?


## ❓ FAQ

**Q: How do I specifically target Department of Defense (DOD) contracts?**
To target DOD contracts, include `DEPARTMENT_ID:"9700"` or `AGENCY_CODE:"9700"` in your `sQuery` parameter when using the `search_contracts` tool.

**Q: Can I paginate through large sets of contract results?**
Yes. The `search_contracts` tool supports a `start` parameter. Results are returned in batches of 10, so you can increment the start number (e.g., 10, 20, 30) to see more records.

**Q: What search syntax should I use for the sQuery parameter?**
The `search_contracts` tool uses the standard FPDS Atom Feed search syntax. You can search by keywords, or use specific fields like `VENDOR_NAME:"Example Corp"` or `PIID:"ContractID"`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dod-contracts-fpds](https://vinkius.com/mcp/dod-contracts-fpds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DOD Contracts (FPDS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dod-contracts-fpds` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DOD Contracts (FPDS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dod-contracts-fpds": {
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

# DailyMed Drug Labels MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dailymed-drug-labels)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Universal drug label intelligence — search official FDA labels and packaging via AI.

## Description
Equip your AI agent with the official source for FDA-published drug labels through the **DailyMed** MCP server. This integration provides real-time access to the National Library of Medicine's (NLM) database of Structured Product Labeling (SPL). Your agent can search for drug labels by name, retrieve detailed packaging information (including NDC codes and NDC history), and explore official prescribing information. Whether you are auditing medication packaging, researching regulatory labeling history, or verifying NDC identifiers, your agent acts as a dedicated regulatory specialist through natural conversation.

### What you can do

- **Label Search** — Find official FDA drug labels by medication name or keyword.
- **NDC Lookup** — Retrieve detailed packaging and labeling information for specific NDC codes.
- **History Tracking** — Explore the historical records of NDC changes and packaging updates.
- **Packaging Auditing** — Summarize official packaging details for pharmaceutical inventory and compliance.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying official drug labels from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Pharmaceutical Logistics Teams** — verify NDC codes and packaging history for inventory management.
- **Regulatory Affairs Specialists** — access the official record of FDA-published drug labels.
- **Healthcare Providers** — quickly find prescribing information and official labels for patient care.
- **Health Tech Developers** — integrate official FDA labeling data into their AI-powered medical tools.


## Available Tools (3)
- **get_drug_details**: Get detailed info for a drug
- **list_drug_classes**: List drug classes
- **search_drugs**: Search for drugs by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DailyMed Drug Labels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for official FDA labels for 'metformin'."

**🤖 AI Agent:**
> Searching DailyMed... I've found several official labels for Metformin from various manufacturers. Would you like to see the specific NDC codes or prescribing information for one of them?

---

**👤 You:**
> "Get packaging details for NDC '0002-3227-30'."

**🤖 AI Agent:**
> Retrieving NDC details... This code refers to Prozac (Fluoxetine) 20mg capsules in a 30-count bottle. The labeler is Eli Lilly and Company. I can provide the full history of this NDC if you need.

---

**👤 You:**
> "Show me the history of changes for NDC '0006-0910-28'."

**🤖 AI Agent:**
> Fetching historical records... I've retrieved the update history for this NDC. It includes changes to the packaging layout and updates to the prescribing information over the last 5 years. Would you like a summary of the most recent change?


## ❓ FAQ

**Q: What is an NDC code?**
NDC stands for National Drug Code. It is a unique 10-digit or 11-digit, 3-segment number used in the US to identify human drugs.

**Q: Can I search for labels by generic name?**
Yes! The `search_drug_labels` tool accepts drug names, which can be either brand names or generic names. It will return all matching official labels.

**Q: Does this include the history of packaging changes?**
Yes. The `get_ndc_history` tool specifically retrieves the record of changes and updates associated with a particular National Drug Code.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dailymed-drug-labels](https://vinkius.com/mcp/dailymed-drug-labels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DailyMed Drug Labels** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dailymed-drug-labels` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DailyMed Drug Labels** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dailymed-drug-labels": {
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

# Atlan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/atlan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Search and discover data assets, business glossaries, classifications, policies, and personas directly via your AI agent.

## Description
Connect your **Atlan** workspace to any AI agent and empower it to become a master data steward. By linking the leading Active Metadata Management platform with agents, you gain conversational governance and instant data cataloging capabilities on demand.

### What you can do

- **Asset Search** — Query your entire connected data ecosystem (tables, dashboards, columns) via natural text to discover lineage and trusted data instantly
- **Business Glossaries** — Retrieve organizational glossaries containing verified business terms, acronyms, and trusted definitions used by your enterprise
- **Classifications & Policies** — List active data classifications (like PII or Confidential tags) and configured sharing purposes (data policies) across the estate
- **Users & Personas** — Inspect registered users and configured access control profiles (Personas) aligned to specific business roles

### How it works

1. Subscribe to this secure MCP Server
2. Provide your Atlan API URL and API Key
3. Start managing data governance naturally from Claude, Cursor, or any compatible AI client

Your AI agent gains deep context about what data means, where it lives, and who owns it.

### Who is this for?

- **Data Stewards** — audit metadata completeness, glossaries, and PII tags systematically through conversation
- **Data Analysts** — quickly discover the right verified tables and dashboards before starting a project
- **Enterprise AI Teams** — ground other LLMs and agents in real metadata context by pulling exact definitions of business KPIs
- **Security & Governance** — inspect broad access personas and data-sharing purposes seamlessly


## Available Tools
- **search_assets**: Search for data assets in the Atlan Data Catalog
- **list_glossaries**: List all business glossaries in Atlan
- **list_classifications**: ) configured in Atlan for data governance purposes.

List all classifications defined in Atlan
- **list_purposes**: List all Atlan Purposes
- **list_personas**: List all Atlan Personas
- **list_users**: List all users in the Atlan workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Atlan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for any data assets related to 'churn prediction'."

**🤖 AI Agent:**
> I searched the Atlan catalog and found 5 matching assets for 'churn prediction': 1 Snowflake schema (`prod_churn_logs`), 2 Looker dashboards summarizing retention, and 2 verified glossaries defining the calculation metrics. What should I explore further?

---

**👤 You:**
> "What business glossaries do we have configured in our metadata?"

**🤖 AI Agent:**
> Your organization operates 4 primary active glossaries on Atlan: `Core Finance KPIs`, `Marketing Attribution Rules`, `Engineering Data Contracts`, and `Regulatory Policies`. Their respective term counts vary per domain structure.

---

**👤 You:**
> "List all security classifications defined across our catalogs."

**🤖 AI Agent:**
> There are 7 active classification tags in Atlan currently utilized across your assets. Notable ones include `GDPR_Sensitive`, `Confidential_Tier_1`, and `Public_Domain`. I can identify the specific tags shielding individual table rows if directed.


## ❓ FAQ

**Q: Can my AI search for a specific dashboard or data table by keyword?**
Yes. Ask the agent to perform an asset search using a natural phrase like 'Q3 revenue report' or 'customer addresses table'. The agent triggers Atlan's semantic asset search, returning linked objects across all connected BI and database sources.

**Q: Are custom Atlan Classifications and Tags exposed to the AI?**
Yes. The agent can list all organizational classifications configured in Atlan (e.g., Sensitive, Restricted, CCPA). This lets the AI contextualize whether the assets it discovers are safe to be shared globally or subject to governance restrictions.

**Q: Can the agent modify or write back metadata to Atlan?**
No. This MCP integration focuses strictly on safe discovery and organizational governance retrieval (queries). It guarantees your metadata catalogues remain pristine, acting purely as an active lookup augmentation tool for your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/atlan](https://vinkius.com/mcp/atlan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Atlan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `atlan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Atlan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "atlan": {
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

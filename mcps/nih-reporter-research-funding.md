# NIH RePORTER (Research Funding) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nih-reporter-research-funding)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access the NIH RePORTER database to search for research projects, funding details, and associated publications.

## Description
Connect to the **NIH RePORTER** (Research Portfolio Online Reporting Tools) to explore the vast landscape of NIH-funded research. This server allows AI agents to query project metadata, funding amounts, principal investigators, and publication records directly from the official government database.

### What you can do

- **Project Discovery** — Search for NIH grants and projects using criteria like fiscal years, PI names, organization names, and project numbers.
- **Funding Analysis** — Retrieve specific award amounts and filter research by agency (e.g., NIGMS, NIAID) or award ranges.
- **Publication Tracking** — Find scientific publications linked to specific NIH applications or core project numbers using PubMed IDs.
- **COVID-19 Research** — Filter projects specifically related to COVID-19 responses and supplemental funding.
- **Advanced Filtering** — Use text searches, date ranges, and organizational matching to find precise research data.

### How it works

1. Subscribe to this server
2. This is a public data service; no private API key is required for standard access, but you can configure your connection to start querying immediately.
3. Start analyzing the NIH research portfolio from Claude, Cursor, or any MCP-compatible client.

### Who is this for?

- **Academic Researchers** — quickly find related work, funding history for specific labs, or publication outputs of NIH grants.
- **Data Scientists** — aggregate funding trends and research outputs for bibliometric or policy analysis.
- **Grant Writers & Administrators** — research successful grant examples and funding patterns within specific institutions or fields.


## Available Tools (2)
- **search_projects**: Use this to find grants, funding amounts, PIs, and organizations.

Search for NIH projects based on specified criteria
- **search_publications**: Search for publications associated with NIH projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NIH RePORTER (Research Funding)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for NIH projects led by 'Anthony Fauci' in fiscal year 2020."

**🤖 AI Agent:**
> I've found several projects for Anthony Fauci in 2020. Notable entries include research on 'Infectious Diseases' and 'Immune Regulation' with Application IDs like 9876543. Would you like the funding details for these?

---

**👤 You:**
> "Find all publications associated with core project number R01AI123456."

**🤖 AI Agent:**
> Searching publications for R01AI123456... I found 12 publications. Titles include 'Novel Mechanisms of Viral Entry' and 'T-cell Response in Chronic Infection'. Would you like the PubMed IDs for these?

---

**👤 You:**
> "List active NIH grants for 'Harvard University' with an award amount over $1,000,000."

**🤖 AI Agent:**
> I've retrieved active grants for Harvard University exceeding $1M. There are 15 projects matching this criteria, including large-scale genomic studies and clinical trial infrastructures. Should I list the PIs for these projects?


## ❓ FAQ

**Q: How can I find all NIH grants awarded to a specific university?**
Use the `search_projects` tool and provide the university name in the `org_names` array. You can also refine the search by adding `fiscal_years` to see awards for a specific period.

**Q: Can I see which publications resulted from a specific NIH project number?**
Yes! Use the `search_publications` tool and enter the project identifier in the `core_project_nums` field. The agent will return a list of associated PubMed records.

**Q: Is it possible to filter research projects by funding amount?**
Absolutely. The `search_projects` tool includes an `award_amount_range` parameter where you can specify `min_amount` and `max_amount` to find projects within your budget criteria.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nih-reporter-research-funding](https://vinkius.com/mcp/nih-reporter-research-funding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NIH RePORTER (Research Funding)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nih-reporter-research-funding` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NIH RePORTER (Research Funding)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nih-reporter-research-funding": {
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

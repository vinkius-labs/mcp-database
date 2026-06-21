# NIH RePORTER (Research Funding) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nih-reporter-research-funding)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nih-reporter-research-funding-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nih-reporter-research-funding-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **NIH RePORTER (Research Funding)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nih-reporter-research-funding](https://vinkius.com/mcp/nih-reporter-research-funding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

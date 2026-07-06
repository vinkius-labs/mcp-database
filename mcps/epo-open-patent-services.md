# EPO Open Patent Services MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epo-open-patent-services)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search global patents — audit bibliographic and legal data via AI.

## Description
Empower your AI agent to orchestrate your entire intellectual property research and patent auditing workflow with **EPO Open Patent Services (OPS)**, the authoritative source for European and global patent data. By connecting the EPO OPS API to your agent, you transform complex patent searches into a natural conversation. Your agent can instantly retrieve bibliographic metadata, audit legal statuses, and identify applicants without you ever touching a patent portal. Whether you are conducting competitive intelligence or managing corporate IP constraints, your agent acts as a real-time patent consultant, ensuring your data is always verified and precise.

### What you can do

- **Patent Auditing** — Search for thousands of published patents and retrieve high-resolution metadata, including titles, applicants, and publication dates.
- **Legal Oversight** — Audit the current legal status of any patent publication to understand the administrative reach of IP rights instantly.
- **Bibliographic Discovery** — Query detailed bibliographic data for specific Doc IDs to assist in deep-dive archival classification.
- **Data Intelligence** — Retrieve unique patent identifiers and applicant information to maintain strict organizational control over IP data.
- **Operational Monitoring** — Check API status to ensure your patent research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your EPO Consumer Key and Consumer Secret
3. Start managing your IP intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Patent Attorneys & Analysts** — monitor patent filings and retrieve official metadata straight from your workflow.
- **IP Researchers** — verify legal statuses and audit applicant patterns without manual searching.
- **R&D Leads** — perform rapid audits of competitive patents and identify relevant technology markers through natural language.
- **Operations Leads** — automate patent data querying to orchestrate cross-functional innovation teams smoothly.


## Available Tools (4)
- **search_epo_patents**: Search for published patents in the EPO database
- **check_api_status**: Check if the EPO Open Patent Services are operational
- **get_patent_bibliographic**: Get full bibliographic metadata for a specific patent by Doc ID
- **get_patent_legal_status**: Check the current legal status of a patent publication


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EPO Open Patent Services** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for patents related to 'electric vehicles' using EPO OPS."

**🤖 AI Agent:**
> I've retrieved several patents related to electric vehicles! Notable entries include innovations in battery management and charging infrastructure. Would you like the full bibliographic metadata or the legal status for any of these records?

---

**👤 You:**
> "What is the legal status of patent 'EP1234567'?"

**🤖 AI Agent:**
> I've retrieved the legal status for EP1234567! It is currently identified as 'Granted' and was last updated on [Date]. I can assist you with the full history of administrative markers for this publication if you'd like.

---

**👤 You:**
> "Get bibliographic details for Doc ID 'US20230000001'."

**🤖 AI Agent:**
> I've retrieved the bibliographic metadata for US20230000001! It is a patent titled [Title] by applicant [Applicant]. I can provide the abstract and classification markers to help you identify it in your workflow.


## ❓ FAQ

**Q: How do I find my EPO Credentials?**
Register for an account at the [**EPO OPS developer portal**](https://developers.epo.org/), create an application, and you will receive your Consumer Key and Consumer Secret. Copy and paste them below.

**Q: Does it support legal status checks?**
Yes. The `get_patent_legal_status` tool retrieves the current administrative and legal status metadata for specified patent publications.

**Q: What format is required for Doc IDs?**
The API uses standard EPODOC format (e.g., EP1234567) for patent identifiers across all retrieval tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epo-open-patent-services](https://vinkius.com/mcp/epo-open-patent-services)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EPO Open Patent Services** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `epo-open-patent-services` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EPO Open Patent Services** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "epo-open-patent-services": {
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

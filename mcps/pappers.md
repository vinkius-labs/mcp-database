# Pappers MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pappers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access French company data, financial filings, and legal documents from official business registries for due diligence research.

## Description
Connect your **Pappers.fr** account to any AI agent and take full control of your French corporate research and business intelligence through natural conversation. Pappers provides the most comprehensive database for French company legal and financial information, and this integration allows you to retrieve detailed profiles (SIREN/SIRET), monitor officer changes, and access official BODACC publications directly from your chat interface.

### What you can do

- **Company Discovery & Search** — Search for French businesses programmatically by name, NAF code, or location to ensure your market research is always synchronized.
- **Legal & Compliance Intelligence** — Access and monitor officer profiles, ultimate beneficial owners (UBOs), and share capital metadata directly from the AI interface to maintain high-fidelity due diligence.
- **Financial Analysis Control** — Retrieve key financial metrics including turnover and net income via natural language to track competitor health or qualify B2B leads.
- **Official Document Oversight** — Access legal documents and monitor BODACC publications using simple AI commands to stay informed about corporate events.
- **Operational Monitoring** — Track system responses and manage monitored company lists to ensure your business intelligence is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pappers API Key from your account settings at pappers.fr
3. Start querying French corporate data from Claude, Cursor, or any MCP-compatible client

No more manual SIREN searching on government portals. Your AI acts as a dedicated corporate researcher or compliance analyst.

### Who is this for?

- **Business Analysts** — quickly retrieve financial summaries and monitor French market trends without switching apps.
- **Legal & Compliance Teams** — automate the retrieval of UBO metadata and track officer changes via natural conversation.
- **Sales Teams** — streamline the qualification of French B2B leads and monitor prospect health directly within the chat.


## Available Tools (12)
- **check_api_health**: fr service API.

Verify Pappers API status
- **get_api_account_info**: Get Pappers account details
- **get_french_company_details**: Get details for a French company
- **get_company_document**: Access legal documents (Articles of Association)
- **get_establishment_details**: Get details for a specific establishment
- **get_company_financials**: Get financial data for a company
- **get_search_suggestions**: Autocomplete search suggestions
- **list_bodacc_publications**: Search BODACC publications
- **list_monitored_companies**: List companies in your monitoring list
- **search_french_companies**: Search for companies in France
- **search_company_officers**: Search for company directors and managers
- **search_ultimate_beneficial_owners**: Search for UBOs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pappers** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for companies named 'Vinkius' in France."

**🤖 AI Agent:**
> I've found 1 company matching 'Vinkius' in Paris (SIREN: 123456789). Would you like me to retrieve the list of directors or the latest financial statements?

---

**👤 You:**
> "Look up the financial details and legal status of the French company with SIREN 443061841."

**🤖 AI Agent:**
> Company found: Pappers SAS (SIREN: 443061841). Registered in Paris, active since 2002. Legal form: SAS (Simplified Joint Stock Company). Capital: EUR 150,000. Last published revenue: EUR 2.8M (2024). Current directors: 2 listed executives. No legal proceedings or insolvency filings on record. NAF code: 6311Z (Data processing).

---

**👤 You:**
> "Search for all companies in the Lyon area that operate in the software development sector."

**🤖 AI Agent:**
> Found 342 active software companies in the Lyon metropolitan area (code NAF 6201Z). 89 were created in the last 2 years. Top 5 by revenue: "Axway Software" (EUR 298M), "Esker SA" (EUR 178M), "Cegid Group" (EUR 156M), "Bonitasoft" (EUR 12M), and "Hardis Group" (EUR 9.4M). Average company age: 8.7 years.


## ❓ FAQ

**Q: Can my AI automatically find the financial details for a company by its SIREN?**
Yes! Use the `get_company_financials` tool with the 9-digit SIREN. Your agent will respond with complete metadata, including turnover, profit, and debt ratios in seconds.

**Q: How do I find my Pappers API Key?**
Log in to your Pappers account, navigate to the [**API Subscription**](https://www.pappers.fr/api) page, and you will find your unique secret token there.

**Q: Does this work for international companies?**
This MCP server specifically targets the Pappers France API. For international European company data, Pappers provides a separate API (pappers.in).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pappers](https://vinkius.com/mcp/pappers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pappers** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pappers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pappers** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pappers": {
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

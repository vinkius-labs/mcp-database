# CNJ (Datajud API Pública) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cnj-datajud-api-publica)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access the Brazilian National Council of Justice (CNJ) Datajud API to query judicial processes, procedural classes, and court organs across Brazil.

## Description
Connect to the **CNJ Datajud Public API** to perform deep searches across the Brazilian judicial system. This server allows AI agents to retrieve detailed metadata about lawsuits, court movements, and procedural history directly from the official national database.

### What you can do

- **Search by CNJ Number** — Retrieve full details of a specific lawsuit using its unique unformatted numbering and the target court alias.
- **Class & Organ Filtering** — Find processes categorized by their Procedural Class (TPU) and specific Court Organ codes.
- **Advanced Elasticsearch Queries** — Execute complex searches using the full power of Elasticsearch Query DSL to filter by dates, parties, or specific metadata fields.
- **Court Coverage** — Access data from various courts including TRFs, TJs, TST, and more via their respective API aliases.

### How it works

1. Subscribe to this server
2. Enter your CNJ Datajud API Key
3. Start querying the Brazilian judicial database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — Quickly check the status and history of lawsuits without manual portal navigation.
- **Compliance Teams** — Automate background checks and legal risk assessments using official government data.
- **Researchers & Analysts** — Perform bulk queries and advanced data extraction for legal statistics and trends.


## Available Tools
- **search_processes_advanced**: Execute an advanced Elasticsearch query against the Datajud API
- **search_processes_by_class_and_organ**: Search processes by Procedural Class and Court Organ
- **search_process_by_number**: g., api_publica_trf1, api_publica_tjsp).

Search for a specific judicial process by its CNJ number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CNJ (Datajud API Pública)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for process number 50012345620234036100 in the TRF3 public API."

**🤖 AI Agent:**
> I found the process in TRF3. It is a 'Procedural' class lawsuit currently assigned to the 1st Federal Court of São Paulo. The last movement was 'Conclusion for Sentence' on October 12th.

---

**👤 You:**
> "List 5 processes from TJDFT with class code 1116 and organ code 12345."

**🤖 AI Agent:**
> I've retrieved 5 processes from TJDFT matching those criteria. The results include processes related to 'Tax Execution' in the specified organ. Would you like to see the details of the most recent one?

---

**👤 You:**
> "Run an advanced search in TST for processes moved in the last 7 days."

**🤖 AI Agent:**
> I found 12 processes with movements in the last week. Most are related to 'Labor Appeals'. I can list their numbers and main subjects for you.


## ❓ FAQ

**Q: How do I find a process if I only have the CNJ number?**
Use the `search_process_by_number` tool. You will need the unformatted digits of the process and the specific court alias (e.g., `api_publica_tjsp` for São Paulo State Court).

**Q: Can I list multiple processes from a specific court organ?**
Yes, use `search_processes_by_class_and_organ`. Provide the court alias, the procedural class code, and the organ code. You can also control the result size and use pagination.

**Q: What is the 'Advanced Search' tool for?**
The `search_processes_advanced` tool allows you to send a raw Elasticsearch query body. This is useful for complex filtering that isn't covered by standard search tools, such as filtering by specific dates or nested metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnj-datajud-api-publica](https://vinkius.com/mcp/cnj-datajud-api-publica)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CNJ (Datajud API Pública)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cnj-datajud-api-publica` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CNJ (Datajud API Pública)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cnj-datajud-api-publica": {
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

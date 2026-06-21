# Senado Federal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/senado-federal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access real-time data from the Brazilian Federal Senate — track legislative proposals, senator profiles, and mandate histories.

## Description
Connect to the **Senado Federal** Open Data API to monitor the Brazilian legislative process directly through your AI agent. Get transparency and deep insights into the upper house of the National Congress.

### What you can do

- **Senator Profiles** — List current senators, those on leave, and access detailed metadata including party affiliations and historical positions.
- **Legislative Proposals (Matérias)** — Search for specific proposals, track their current status, and view the complete history of movements and actions.
- **Rapporteur Tracking** — Identify which senators are assigned as rapporteurs for specific bills and proposals.
- **Legislative History** — Explore current and historical legislatures to understand the evolution of Brazilian law.
- **Mandate Analysis** — Inspect the full history of mandates and political roles held by any parliamentarian.

### How it works

1. Subscribe to this server
2. Use 'PUBLIC' or your preferred identifier as the access key
3. Start querying the Brazilian Senate database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly verify senator backgrounds and the status of controversial bills.
- **Legal Professionals** — track the progress of legislative changes that affect specific sectors.
- **Civic Tech Developers** — integrate official government data into applications with ease.


## Available Tools (21)
- **get_comissao_composicao**: Get current members of a committee
- **get_comissao**: Get detailed information about a specific committee
- **get_legislatura_atual**: Get details of the current legislature
- **get_legislatura**: Get details of a specific legislature
- **get_materia_movimentacoes**: Get history of actions on a proposal
- **get_materia_relatorias**: Get rapporteurs assigned to a proposal
- **get_materia**: Get detailed information about a specific proposal
- **get_senador_cargos**: Get positions held by a senator
- **get_senador_filiacoes**: Get party affiliations of a senator
- **get_senador_mandatos**: Get mandates held by a senator
- **get_senador**: Get detailed information about a specific senator
- **get_votacao**: Get details of a specific vote
- **list_agenda_reuniao**: List scheduled committee meetings
- **list_agenda_sessao**: List scheduled sessions
- **list_comissoes**: List all committees
- **list_legislaturas**: List all legislatures
- **list_materias_atualizacoes**: List recently updated legislative proposals
- **list_materias_tipos**: g., PL, PEC).

List types of legislative proposals
- **list_senadores_afastados**: List senators currently on leave
- **list_senadores_atual**: List senators currently in office
- **list_votacoes**: List recent votes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Senado Federal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all senators currently in office."

**🤖 AI Agent:**
> I've retrieved the list of senators currently in office. There are 81 active senators, including names like [Senator Name] from [Party/State]. Would you like details on a specific one?

---

**👤 You:**
> "Get the details and summary of legislative proposal ID 150000."

**🤖 AI Agent:**
> Fetching proposal 150000... This is a [Type] proposal regarding [Subject]. Its current status is [Status] and the summary states: '[Summary Text]'.

---

**👤 You:**
> "Show the party affiliation history for senator ID 500."

**🤖 AI Agent:**
> Analyzing affiliation history for senator 500... They are currently with [Current Party] and were previously affiliated with [Past Party 1] and [Past Party 2].


## ❓ FAQ

**Q: Can I see the history of actions and movements for a specific legislative proposal?**
Yes! Use the `get_materia_movimentacoes` tool with the Proposal ID (CodigoMateria). It will return the full chronological list of actions taken on that bill.

**Q: How do I find out which senators are currently on leave?**
Simply run the `list_senadores_afastados` tool. It retrieves the list of Brazilian senators who are currently not in active office due to leave.

**Q: Is it possible to check the historical positions held by a senator?**
Yes, use the `get_senador_cargos` tool with the Senator ID. It provides a detailed list of current and past positions held within the Senate and other bodies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/senado-federal](https://vinkius.com/mcp/senado-federal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Senado Federal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `senado-federal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Senado Federal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "senado-federal": {
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

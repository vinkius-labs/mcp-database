# Tactile CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tactile-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI to Tactile CRM. Query companies, read contact details, and evaluate your sales opportunities and pipelines natively from the terminal.

## Description
Extend the reach of your **Tactile CRM** databases directly into your AI conversational flow utilizing this official Vinkius MCP connector. By granting your LLM localized parsing privileges, you enable it to operate as an intelligent sales assistant that can explore rich business metadata, track sales progression, and summarize unstructured internal notes strictly without relying on graphical CRM interfaces.

### What you can do

- **Client & Corporate Lookups** — Investigate CRM records retrieving specific macro structures invoking `list_companies` and pinpoint specific organizational data operating `get_company_details`.
- **Contact Identification** — Sweep active employee registers querying `list_contacts` and securely extract direct lead data mapping them dynamically with `get_contact_details`.
- **Pipeline Discovery** — Analyze sales cycle projections seamlessly using `list_opportunities` and drill into individual contract values utilizing `get_opportunity_details`.
- **Activity & Note Audits** — Programmatically capture unstructured comments analyzing metadata tracks applying `list_notes` and log engagement events executing `list_activities`.

### How it works

1. Associate the active Tactile CRM integration environment securely over your prompt terminal interface.
2. Accurately assign your corporate `TACTILE_SUBDOMAIN` and specific access matrix (`TACTILE_API_KEY`) obtained from Account Settings > Integrations.
3. Instruct your artificial assistant logically: "Search our CRM companies for 'Acme Corp', evaluate their most recent activities, and retrieve the primary contact email from our pipelines."

### Who is this for?

- **B2B Account Executives** — Instantly review pre-meeting client summaries pulling unformatted notes cleanly into the conversation window bypassing complex web portals.
- **Sales Operation Analysts** — Cross-reference opportunities tracking active funnels programmatically inspecting structural data parameters natively.
- **Customer Success Managers** — Assess real-time organizational footprints logging activities verifying specific company details via simple conversational text evaluations.


## Available Tools (9)
- **list_opportunities**: Lists all sales opportunities (deals) in the pipeline
- **get_opportunity_details**: Retrieves details for a specific sales opportunity
- **list_activities**: Lists recent CRM activities (tasks, calls, emails)
- **list_pipelines**: Lists available sales pipelines
- **list_notes**: Lists general CRM notes
- **list_companies**: Lists all companies (organizations) in the Tactile CRM
- **get_company_details**: Retrieves details for a specific company
- **list_contacts**: Lists all individual contacts (people) in the CRM
- **get_contact_details**: Retrieves details for a specific individual contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tactile CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the list of sales pipelines and extract the basic contact details for the latest three companies created in the CRM."

**🤖 AI Agent:**
> Retrieving data via 'list_pipelines' and 'list_companies' securely...
Found Companies: 'AlphaTech', 'BetaCorp', 'GammaInc'.
Evaluating specific variables natively via 'get_company_details'...

**Company Meta-Details**:
- **AlphaTech**: Tech Sector, 5 Active Deals logged (checking 'list_opportunities').
- **BetaCorp**: Manufacturing, 2 unresolved interaction activities.
- **GammaInc**: Finance, latest Note: "Wait for Q3 budget approval".

---

**👤 You:**
> "List all open support tickets related to 'login issues'."

**🤖 AI Agent:**
> Interrogating Tactile CRM limits ('list_tickets')...
Found 2 open support entities matching 'login issues':
1. Ticket #1024: 'Cannot access dashboard' (Priority: High)
2. Ticket #1055: 'SSO failure on mobile' (Priority: Medium)

---

**👤 You:**
> "Create a new contact constraint for 'John Doe' assigned to the 'Enterprise' tag."

**🤖 AI Agent:**
> Executing `create_contact` operation in Tactile...
Contact 'John Doe' successfully inserted.
Added organizational tag 'Enterprise'.
New native ID: `cont-9941`.


## ❓ FAQ

**Q: Is the integration read-only?**
Yes. All tools (list_companies, list_contacts, list_opportunities, etc.) are read-only queries. They cannot modify, create, or delete any CRM records.

**Q: What is the TACTILE_SUBDOMAIN?**
It's the unique prefix of your Tactile CRM URL (e.g., if your URL is `acme.tactilecrm.com`, the subdomain is `acme`). You can find it in the address bar when logged in.

**Q: What data can the agent access?**
Companies, contacts, opportunities with pipeline stages, notes, and activities. The scope is determined by the permissions of the API key you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tactile-crm](https://vinkius.com/mcp/tactile-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tactile CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tactile-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tactile CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tactile-crm": {
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

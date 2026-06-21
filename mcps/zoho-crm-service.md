# Zoho CRM Service MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-service)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage support cases and knowledge base solutions — customer service operations through Zoho CRM.

## Description
Connect **Zoho CRM** to any AI agent — manage your entire CRM without switching tabs.

### What you can do
- **Leads** — Search and create leads with source and status tracking
- **Contacts** — Find and create contacts linked to accounts
- **Accounts** — Search companies and organizations
- **Deals** — Search, create, and track deals through pipeline stages
- **Notes** — Create notes attached to any CRM record
- **Generic List** — Query any Zoho CRM module directly

### Who is this for?
- **Sales Reps** — CRM at your fingertips through AI
- **BDRs** — Quickly qualify and create leads
- **Sales Managers** — Pipeline visibility and deal insights
- **Support Teams** — Access contact and account data seamlessly


## Available Tools (7)
- **zoho_create_case**: Subject is required. Status: New, Assigned, On Hold, Closed. Priority: High, Medium, Low. Case_Origin: Phone, Email, Web, Chat, Forum, Twitter. Case_Reason: Installation, Performance, Feature Request, etc. Use when logging a new customer issue or support request.

Create a new support case in Zoho CRM with subject, priority, origin channel, reason, and description
- **zoho_create_solution**: Solution_Title, Question, and Answer are required. Status: Draft, Reviewed, Published. Published solutions are accessible in the self-service knowledge base. Use when the user wants to document a new solution, answer a FAQ, or create a reference article.

Create a new knowledge base article in Zoho CRM with title, question, answer, and publish status
- **zoho_list_cases**: Returns case subject, status (New/Assigned/Closed), priority (High/Medium/Low), case origin (Phone/Email/Web/Chat), case reason, and owner. Cases track customer support issues. Use when the user asks about open support cases, case workload, or support queue status.

List support cases in Zoho CRM with subject, status, priority, origin channel, and assigned owner
- **zoho_list_solutions**: Solutions are knowledge base articles with a Question and Answer format. Returns title, status (Draft/Reviewed/Published), and content. Use when the user asks about existing KB articles, wants to find documented solutions, or needs to audit the knowledge base.

List knowledge base solutions/articles in Zoho CRM with title, question, status, and review information
- **zoho_search_cases**: Returns matching cases with subject, status, priority, origin, and owner. Use when the user wants to find a specific support case, look up a customer issue, or check the status of a reported problem.

Search Zoho CRM support cases by subject or keyword to find specific customer issues
- **zoho_search_solutions**: Returns matching KB articles with title, status, and content. Use when the user asks "do we have a KB article about X?" or wants to find existing documentation before creating a new solution.

Search the Zoho CRM knowledge base for solutions/articles by keyword to find documented answers to common issues
- **zoho_update_case**: Only specified fields change. Common operations: set Status to "Closed" when resolved, escalate Priority to "High", or update Subject for clarity. Use when a case progresses or needs correction.

Update an existing Zoho CRM case — change status, priority, or subject to reflect resolution progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM Service** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from web form"

**🤖 AI Agent:**
> 👥 **Leads from Web Form**
| Name | Email | Company | Status |
|---|---|---|---|
| John Smith | john@acme.com | Acme Corp | New |
| Maria Garcia | maria@beta.io | Beta Inc | Contacted |

---

**👤 You:**
> "Create a deal: Enterprise Plan $25,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Plan
- Amount: $25,000
- Stage: Qualification
- Closing: 2024-03-30


## ❓ FAQ

**Q: What Zoho CRM data can I access?**
Leads, Contacts, Accounts, Deals, Notes, and any custom module. All data respects your Zoho CRM permissions.

**Q: How does authentication work?**
Uses Zoho OAuth 2.0 with a refresh token. Create a Self Client in the Zoho API Console, generate a refresh token, and provide Client ID, Client Secret, and Refresh Token.

**Q: Does it support multi-region Zoho?**
Yes! Set your API domain: zohoapis.com (US), zohoapis.eu (EU), zohoapis.in (India), zohoapis.com.au (Australia), zohoapis.jp (Japan).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-service](https://vinkius.com/mcp/zoho-crm-service)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho CRM Service** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-crm-service` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho CRM Service** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-crm-service": {
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

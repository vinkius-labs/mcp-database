# Zoho CRM Admin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-admin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Zoho CRM users, roles, profiles, layouts, territories, and tags — complete admin control through conversation.

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


## Available Tools
- **zoho_get_user**: Returns full profile: name, email, role, profile (permissions), locale, timezone, created date, and last activity. Use to get detailed info about a specific team member or administrator.

Get complete details of a specific Zoho CRM user by ID, including role, profile, locale, and activity info
- **zoho_list_layouts**: Returns layout name, status (active/inactive), and section structure. Layouts define how the record form appears in the UI — which fields are shown, their grouping into sections, and display order. Different layouts can be assigned to different profiles. Use when the user asks about form configuration or field arrangement.

List page layouts for a Zoho CRM module, showing the form structure with sections and field arrangement
- **zoho_list_profiles**: Returns profile name, description, and whether it is the default. Profiles are permission sets controlling module access, field-level visibility, and feature availability (e.g., Administrator, Standard, Marketing). While roles control data visibility, profiles control feature access. Use to audit permissions or understand what different user groups can do.

List Zoho CRM profiles (permission sets) that control what features, modules, and actions users can access
- **zoho_list_roles**: Returns role name, reporting role (parent in the hierarchy), and description. Roles control data visibility — users can see records of their subordinate roles. Use to understand the organizational hierarchy, access control structure, or when the user asks about role assignments.

List all roles in Zoho CRM with their hierarchy structure, showing who reports to whom in the organization
- **zoho_list_tags**: Returns tag name, color, and creator. Tags are user-defined labels for quick categorization and filtering of records (e.g., "VIP", "Urgent", "Follow-up Required"). Use when the user asks about available tags, wants to understand how records are categorized, or needs tag names for filtering.

List all tags available for a Zoho CRM module for record categorization and quick filtering
- **zoho_list_territories**: Returns territory name, manager, parent territory, and description. Territories organize the sales team by geography, product line, or customer segment (e.g., "North America", "Enterprise", "EMEA"). Records can be assigned to territories for routing and reporting. Use when the user asks about sales territories or geographic coverage.

List sales territories in Zoho CRM with territory names, managers, and hierarchy for geographic/segment-based sales organization
- **zoho_list_users**: Returns user name, email, role, profile (permission set), active/inactive status, and timezone. Filter by type: AllUsers, ActiveUsers, DeactiveUsers, AdminUsers. Use when the user asks about team members, needs user IDs for record assignment, or wants to audit CRM access.

List Zoho CRM users with name, email, role, profile, status, and timezone for team management visibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM Admin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-admin](https://vinkius.com/mcp/zoho-crm-admin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho CRM Admin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zoho-crm-admin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho CRM Admin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-crm-admin": {
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

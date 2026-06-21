# Salesforce Sales Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-sales-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage leads, opportunities, accounts, contacts, and your entire sales pipeline through natural conversation with your Salesforce CRM.

## Description
Connect **Salesforce Sales Cloud** to any AI agent — instant access to your CRM data without switching tabs.

### What you can do
- **Leads** — Search, create, update, and qualify leads by name, email, or company
- **Opportunities** — Track deals, update stages, amounts, and close dates
- **Accounts** — Look up company details including revenue, industry, and employees
- **Contacts** — Find contacts by name or email with account associations
- **Activities** — Log calls, meetings, and emails as Tasks linked to records
- **Pipeline** — Get an instant summary of your open pipeline by stage

### Who is this for?
- **Sales Reps** — Save 1-2 hours/day by managing your CRM through conversation
- **SDRs** — Create and qualify leads without leaving your workflow
- **RevOps** — Get pipeline snapshots and deal data instantly
- **Account Executives** — Update opportunities and log activities on-the-go


## Available Tools
- **sf_create_lead**: lastName and company are required fields in Salesforce. Status defaults to "Open - Not Contacted". Once qualified, leads can be converted to Contact + Account + Opportunity in the Salesforce UI. Returns the created lead with its 18-character Salesforce ID.

Create a new lead in Salesforce Sales Cloud with name, company, email, phone, title, and initial status
- **sf_opportunities_by_stage**: Returns deals sorted by amount descending. Standard stages: Prospecting, Qualification, Needs Analysis, Value Proposition, Id. Decision Makers, Perception Analysis, Proposal/Price Quote, Negotiation/Review, Closed Won, Closed Lost. Use for questions like "what deals are in Negotiation?" or "total value of Closed Won this quarter."

Get all Salesforce opportunities at a specific pipeline stage for bottleneck analysis, forecasting, or stage review
- **sf_pipeline_summary**: Returns the number of deals and total monetary value at each stage. Perfect for pipeline health checks, forecasting conversations, and identifying bottleneck stages. Use when the user asks "how is the pipeline?", "what is our total pipeline value?", or "which stage has the most deals?"

Get an aggregate snapshot of the open sales pipeline — deal count and total value per stage for a quick health check
- **sf_log_activity**: Link to a person via whoId (Contact or Lead ID) and/or to a record via whatId (Account or Opportunity ID). Status defaults to "Completed". Priority: High, Normal, Low. Use to log completed calls, meetings, or emails for activity tracking and reporting.

Log a call, meeting, or email as a completed Task in Salesforce linked to a contact, lead, account, or opportunity
- **sf_search_accounts**: Returns account name, industry, annual revenue, number of employees, phone, website, billing city/state/country, and owner. Accounts are the company-level records that contacts and opportunities are linked to. Use when the user asks about a company or needs account-level data.

Search Salesforce accounts (companies) by name to find organizations with industry, revenue, employee count, and location
- **sf_search_contacts**: Returns contact name, email, phone, account name, title, department, and mailing address. Contacts are qualified individuals linked to accounts — different from leads (unqualified prospects). Use when the user asks about a specific customer contact.

Search Salesforce contacts by name or email to find people at customer accounts with title, department, and phone
- **sf_search_leads**: Returns lead name, company, email, phone, title, status (e.g., Open - Not Contacted, Working, Closed - Converted), rating (Hot/Warm/Cold), lead source, and assigned owner. Use when the user wants to find a specific prospect, check lead status, or review unqualified pipeline.

Search Salesforce leads by name, email, or company to find prospective customers in the sales pipeline
- **sf_search_opportunities**: Returns opportunity name, stage (Prospecting/Qualification/Needs Analysis/Value Proposition/Id. Decision Makers/Perception Analysis/Proposal/Negotiation/Closed Won/Closed Lost), amount, close date, probability percentage, and assigned owner. Use for pipeline review, deal lookup, or forecasting queries.

Search Salesforce opportunities by name to find deals with stage, amount, probability, close date, and owner
- **sf_update_lead**: Only specified fields are updated. Common operations: change Status to "Working" or "Closed - Converted", set Rating to Hot/Warm/Cold for prioritization, or update contact details. Requires the 18-character Salesforce ID.

Update an existing Salesforce lead — change status, rating, contact info, or other fields to reflect qualification progress
- **sf_update_opportunity**: Common operations: advance StageName when deal progresses, update Amount after negotiation, push CloseDate when timeline shifts, set StageName to "Closed Won"/"Closed Lost" to close. Only specified fields change.

Update a Salesforce opportunity — advance stage, change amount, update close date, or add notes to reflect deal progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce Sales Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all hot leads from this week"

**🤖 AI Agent:**
> 🔥 **Hot Leads — This Week**

| Name | Company | Email | Status |
|---|---|---|---|
| Sarah Chen | TechCorp Inc | s.chen@techcorp.com | Open - Not Contacted |
| James Wilson | DataFlow | j.wilson@dataflow.io | Working |
| Maria Santos | CloudBase | m.santos@cloudbase.com | Open - Not Contacted |

💡 3 hot leads found. Want me to update any of them?

---

**👤 You:**
> "What does my pipeline look like right now?"

**🤖 AI Agent:**
> 📊 **Pipeline Summary**

| Stage | Deals | Total Value |
|---|---|---|
| Prospecting | 12 | $340,000 |
| Qualification | 8 | $520,000 |
| Negotiation | 5 | $890,000 |
| Closed Won (MTD) | 3 | $215,000 |

💰 Total open pipeline: **$1,750,000** across 25 deals

---

**👤 You:**
> "Create a new lead: John Smith from Acme Corp, john@acme.com"

**🤖 AI Agent:**
> ✅ **Lead Created!**

- **Name:** John Smith
- **Company:** Acme Corp
- **Email:** john@acme.com
- **Status:** Open - Not Contacted
- **ID:** 00Q8Z00001ABC

Want me to assign this lead to a specific owner?


## ❓ FAQ

**Q: What Salesforce data can I access?**
Leads, Opportunities, Accounts, Contacts, Tasks, and aggregate pipeline summaries. All data respects your Salesforce field-level security permissions.

**Q: Can I create and update records?**
Yes! You can create Leads and Tasks, update Leads and Opportunities (stage, amount, close date), and log activities — all through natural conversation.

**Q: How does authentication work?**
Uses OAuth 2.0 Client Credentials flow. You provide your Salesforce Instance URL, Consumer Key, and Consumer Secret from a Connected App. The server handles token exchange and renewal automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-sales-cloud](https://vinkius.com/mcp/salesforce-sales-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesforce Sales Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `salesforce-sales-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesforce Sales Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesforce-sales-cloud": {
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

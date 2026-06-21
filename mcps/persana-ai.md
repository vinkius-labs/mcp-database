# Persana AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/persana-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enrich leads with AI that researches prospects, scores intent signals, and builds personalized outreach sequences automatically.

## Description
Connect your **Persana AI** account to any AI agent and take full control of your outbound sales orchestration and lead intelligence through natural conversation. Persana AI provides a powerful platform for finding deep B2B insights, tracking real-time buying signals (like job changes or funding), and maintaining a high-fidelity sales pipeline.

### What you can do

- **Lead & Account Enrichment** — Retrieve 100+ firmographic data points and professional backgrounds programmatically to ensure your prospecting is always synchronized.
- **Intent & Buying Signal Tracking** — Monitor real-time intent signals and job changes across your target accounts directly from the AI interface to prioritize your outreach.
- **Email Lookup & Verification** — Perform waterfall email verification to ensure high deliverability and accuracy via natural language.
- **Lead List Management** — Access and monitor your organized lead lists and retrieve detailed prospect metadata using simple AI commands.
- **Operational Monitoring** — Track system responses and manage organizational metadata to ensure your sales workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Persana AI Key from your dashboard settings
3. Start enriching leads and tracking signals from Claude, Cursor, or any MCP-compatible client

No more manual signal monitoring or searching through disparate data sources. Your AI acts as a dedicated sales scout or lead intelligence coordinator.

### Who is this for?

- **Sales Development (SDRs)** — quickly retrieve prospect summaries and monitor intent signals without switching apps.
- **Account Executives (AEs)** — automate the tracking of key account changes and prioritize outreach via natural conversation.
- **Growth Marketers** — streamline the retrieval of enriched lead data and monitor organizational health directly within the chat.


## Available Tools
- **enrich_company**: Pass data as a JSON string.

Enrich company data
- **enrich_person**: Pass data as a JSON string.

Enrich person data
- **get_lead_list**: Get specific lead list details
- **get_signals**: Get sales intent signals
- **list_lead_lists**: List all lead lists
- **lookup_email**: Verify and lookup emails
- **create_lead_list**: Create a new lead list
- **delete_lead_list**: Delete a lead list
- **find_job_changes**: Find recent job changes in your target accounts
- **search_people**: Search for people by criteria
- **verify_email**: Verify if an email address is deliverable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Persana AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich the prospect with LinkedIn URL 'https://linkedin.com/in/robert-chen'."

**🤖 AI Agent:**
> I've enriched the profile for Robert Chen. He is the 'VP of Engineering' at 'CloudScale'. I found his verified work email (robert@cloudscale.io) and identified 3 recent buying signals for his organization. Would you like a summary of the organization's growth?

---

**👤 You:**
> "Enrich the professional profile for sarah.chen@meridian.io with company and social data."

**🤖 AI Agent:**
> Profile enriched for sarah.chen@meridian.io. Name: Sarah Chen, VP of Engineering at Meridian Corp (Series B, 180 employees). Location: San Francisco, CA. LinkedIn: 2,400+ connections. Previous: Senior Engineer at DataFlow (3 years). Company revenue: $24M ARR. Tech stack detected: React, AWS, PostgreSQL. Buying signal: Recently posted about scaling infrastructure challenges.

---

**👤 You:**
> "Find all job changes in my target account list from the last 30 days."

**🤖 AI Agent:**
> 23 job changes detected in your target accounts over the last 30 days. Notable moves: James Park joined Acme Corp as CTO (previously VP Eng at TechFlow). Lisa Wang became Head of Product at ScaleUp. 8 new VP-level hires detected across your enterprise accounts. 5 contacts left their companies entirely. These represent high-value outreach opportunities since new decision-makers often evaluate tooling within the first 90 days.


## ❓ FAQ

**Q: Can my AI automatically find the verified email for a prospect by their LinkedIn URL?**
Yes! Use the `enrich_person` tool. Provide the LinkedIn URL, and your agent will respond with complete metadata, including firmographics and waterfall-verified email addresses in seconds.

**Q: How do I find my Persana AI Key?**
Log in to your Persana AI dashboard, navigate to **Settings** > **API Keys**, and you will find your unique secret token there.

**Q: What are 'Intent Signals'?**
Intent signals are real-time alerts about key account activities, such as a company raising a new funding round or a decision-maker starting a new role, allowing for perfectly timed outreach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/persana-ai](https://vinkius.com/mcp/persana-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Persana AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `persana-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Persana AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "persana-ai": {
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

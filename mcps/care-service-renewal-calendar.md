# Care Service Renewal Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-service-renewal-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automated orchestration for service contract renewal timelines, review agendas, and decision checklists.

## Description
This MCP server transforms service contracts and renewal parameters into actionable intelligence. It manages the entire renewal cycle by generating chronological timelines via `get_renewal_calendar`, creating structured meeting agendas with `get_provider_review_agenda`, producing high-priority decision checklists with `get_action_list`, and organizing audit-ready documentation plans with `get_evidence_folder_plan`. It is designed to prevent accidental automatic renewals by tracking notice windows and review milestones.


## Available Tools (4)
- **get_action_list**: Produces a high-priority checklist of "cancel or renew" decisions that are currently active or imminent
- **get_evidence_folder_plan**: Organizes a structured plan for where and how documentation should be stored for audit and decision support
- **get_provider_review_agenda**: Creates a structured meeting agenda for decision owners to evaluate a specific provider performance
- **get_renewal_calendar**: Each object must contain serviceName, expirationDate, and noticeWindowDays.

Generates a chronological timeline of all upcoming critical dates for all provided contracts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Service Renewal Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a renewal calendar for my contracts."

**🤖 AI Agent:**
> Here is your renewal timeline: [Contract A: Expiration Oct 1, Notice Deadline Sept 1; Contract B: Expiration Dec 15, Notice Deadline Nov 15].

---

**👤 You:**
> "What are my most urgent renewal decisions?"

**🤖 AI Agent:**
> You have 2 imminent actions: Renew 'Cloud Services' by Friday or cancel 'Office Supplies' before the notice window closes tomorrow.

---

**👤 You:**
> "Create a review agenda for the software provider including price analysis."

**🤖 AI Agent:**
> Agenda for Software Provider: 1. Performance Review (based on satisfaction notes), 2. Price Analysis (showing a 15% increase from $1000 to $1150), 3. Final Decision.


## ❓ FAQ

**Q: How does the tool help prevent automatic contract renewals?**
The `get_renewal_calendar` tool calculates the exact date to provide notice by subtracting the notice window from the expiration date, ensuring you act before the window closes.

**Q: Can I include price changes in the provider review?**
Yes, when using `get_provider_review_agenda`, you can set the price analysis flag to true to include a detailed breakdown of percentage changes between current and proposed pricing.

**Q: What kind of documentation can I plan for?**
The `get_evidence_folder_plan` tool organizes documentation into Legal, Financial, and Performance tiers to support audits and decision-making.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-service-renewal-calendar](https://vinkius.com/en/ai-agent-connect/care-service-renewal-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Service Renewal Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-service-renewal-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Service Renewal Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-service-renewal-calendar": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

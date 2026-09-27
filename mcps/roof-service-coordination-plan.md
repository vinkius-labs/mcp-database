# Roof Service Coordination Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/roof-service-coordination-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [insurance](../categories/insurance.md)

Synchronize property inspections, contractor quotes, and insurance deadlines into actionable maintenance timelines.

## Description
This MCP server acts as a strategic coordination engine for roof maintenance and repair management. It bridges the gap between visible property symptoms and formal insurance requirements. By using tools like `generate_visit_schedule`, `compare_quote_agendas`, `build_evidence_checklist`, and `calculate_decision_timeline`, users can transform raw inspection data and contractor proposals into structured visit schedules, evidence checklists, and critical decision timelines. It ensures all contractor activities are completed before insurer deadlines to protect claim validity.


## Available Tools (4)
- **build_evidence_checklist**: Generate a checklist of required evidence to support an insurance claim
- **calculate_decision_timeline**: Calculate the critical path and decision buffer relative to the insurer deadline
- **compare_quote_agendas**: Generate an agenda to compare different contractor quotes
- **generate_visit_schedule**: Generate a schedule for contractor visits based on symptoms, reports, and access constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roof Service Coordination Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a leak in my roof and a storm happened last week. My insurer deadline is 2024-12-01. Can you help me plan?"

**🤖 AI Agent:**
> I will use `build_evidence_checklist` to identify what documentation you need from the storm and the leak, and `calculate_decision_timeline` to map out your path before the December 1st deadline.

---

**👤 You:**
> "I have three quotes for my roof repair. How should I evaluate them?"

**🤖 AI Agent:**
> I can use `compare_quote_agendas` to create a comparison agenda that focuses on how each quote addresses your specific roof symptoms.

---

**👤 You:**
> "The contractor can only visit on Mondays. When should they come to meet my insurer deadline of 2024-11-15?"

**🤖 AI Agent:**
> I will use `generate_visit_schedule` to find the best available Mondays that respect your property access and ensure completion before November 15th.


## ❓ FAQ

**Q: How does this tool help with insurance claims?**
It uses `build_evidence_checklist` to identify necessary documentation and `calculate_decision_timeline` to ensure all actions are completed before the insurer's deadline.

**Q: Can I use this to compare different contractor quotes?**
Yes, the `compare_quote_agendas` tool provides a structured way to evaluate proposals based on the specific symptoms reported.

**Q: What information is needed to create a visit schedule?**
You need to provide the observed symptoms, existing inspection reports, available property access windows, and the insurer deadline for `generate_visit_schedule`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/roof-service-coordination-plan](https://vinkius.com/en/ai-agent-connect/roof-service-coordination-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roof Service Coordination Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roof-service-coordination-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roof Service Coordination Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roof-service-coordination-plan": {
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

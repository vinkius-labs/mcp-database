# Incident to Claim Timeline MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/incident-to-claim-timeline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Chronologically sequence insurance incident events, witness statements, and policy milestones into a factual timeline.

## Description
This MCP server provides tools to reconstruct a complete, ordered history of insurance-related data. Use `get_chronological_timeline` to merge incident events, witness statements, notices, and policy milestones into a single chronological sequence. You can also use `summarize_claim_status` to get a narrative of the time elapsed since the incident, `validate_reporting_compliance` to check if a claim was reported within required policy windows, and `filter_timeline_by_type` to isolate specific categories like notices or policy milestones.


## Available Tools (4)
- **summarize_claim_status**: Provides a high-level narrative summary of the time elapsed between the incident and the current status
- **filter_timeline_by_type**: Extracts a subset of the timeline focused on a specific category
- **get_chronological_timeline**: Reconstructs a complete, ordered history of all provided incident-related data points
- **validate_reporting_compliance**: Checks if the claim was reported within the required timeframes defined by policy milestones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Incident to Claim Timeline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a timeline from these events: Incident on 2023-01-01 (Burst Pipe), Policy Effective on 2022-12-01, and Notice sent on 2023-01-05."

**🤖 AI Agent:**
> 1. 2022-12-01: Policy Effective (Policy)
2. 2023-01-01: Burst Pipe (Incident)
3. 2023-01-05: Notice sent (Notice)

---

**👤 You:**
> "Was the claim reported within 3 days of the incident? Incident: 2023-05-10, Notice: 2023-05-12."

**🤖 AI Agent:**
> The claim is Compliant. The notice was reported 2 days after the incident.

---

**👤 You:**
> "Summarize the status for a timeline where the incident was 2023-06-01 and today is 2023-06-10."

**🤖 AI Agent:**
> Total days since incident: 9. The incident occurred 9 days ago.


## ❓ FAQ

**Q: How do I create a chronological sequence of events?**
Use the `get_chronological_timeline` tool by providing the incident events, witness statements, notices, and policy milestones as JSON strings.

**Q: Can I check if a claim was reported on time?**
Yes, use the `validate_reporting_compliance` tool to compare the earliest incident event against the earliest notice based on your specified deadline.

**Q: How can I get a summary of the time elapsed since the incident?**
You can use `summarize_claim_status` with the generated timeline and a target date to receive a narrative summary and total days elapsed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/incident-to-claim-timeline](https://vinkius.com/en/ai-agent-connect/incident-to-claim-timeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Incident to Claim Timeline** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `incident-to-claim-timeline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Incident to Claim Timeline** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "incident-to-claim-timeline": {
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

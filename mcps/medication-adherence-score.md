# Medication Adherence Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/medication-adherence-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Analyzes medication adherence through dosage, timing, and persistence metrics.

## Description
This MCP server provides clinical tools to evaluate how strictly patients follow their medication regimens. It calculates the adherence percentage using `get_adherence_percentage`, assesses timing reliability with `get_timing_consistency`, determines therapy duration via `get_persistence_days`, and identifies clinical urgency through `get_intervention_priority`. It helps clinicians identify high-risk patients based on dosage completion, timing precision, and refill patterns.


## Available Tools (4)
- **get_adherence_percentage**: Calculates the basic ratio of medication uptake relative to the prescription
- **get_intervention_priority**: Identifies the clinical urgency required to contact a patient based on their adherence profile
- **get_persistence_days**: Determines the length of time a patient has stayed on their medication therapy
- **get_timing_consistency**: Evaluates how reliably a patient adheres to the prescribed clock-time for their doses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Medication Adherence Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the adherence rate if 45 doses were taken out of 50 prescribed?"

**🤖 AI Agent:**
> The adherence rate is 90%, which is classified as High Adherence.

---

**👤 You:**
> "How many days has the patient been on medication if the first dose was 2023-01-01 and the last was 2023-01-15?"

**🤖 AI Agent:**
> The patient has been on medication for 15 days.

---

**👤 You:**
> "A patient has an adherence rate of 0.4, a consistency score of 0.5, and a refill gap was detected. What is the priority?"

**🤖 AI Agent:**
> The priority level is Urgent, and the recommended action is immediate clinician outreach.


## ❓ FAQ

**Q: How is the adherence percentage calculated?**
The `get_adherence_percentage` tool calculates the ratio of doses actually taken compared to the total doses prescribed for the period.

**Q: Can I determine if a patient needs immediate intervention?**
Yes, use `get_intervention_priority` to identify clinical urgency based on adherence rates, timing consistency, and refill gaps.

**Q: How does the tool measure timing consistency?**
The `get_timing_consistency` tool compares the scheduled dose times against the actual recorded times to calculate a consistency score and average deviation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/medication-adherence-score](https://vinkius.com/en/ai-agent-connect/medication-adherence-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Medication Adherence Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `medication-adherence-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Medication Adherence Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "medication-adherence-score": {
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

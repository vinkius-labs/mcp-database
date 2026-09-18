# ADHD Medication Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/adhd-medication-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Monitor ADHD medication timing, effectiveness, and coverage gaps using pharmacokinetic modeling.

## Description
This MCP server provides a specialized monitoring system for ADHD medication management. It uses pharmacokinetic modeling to track how different formulations, such as immediate or extended release, impact therapeutic windows. Users can use `log_medication_event` to record doses, `get_medication_coverage` to identify symptom coverage gaps, `analyze_effectiveness` to correlate side effects with peak times, and `suggest_optimization` to receive data-driven recommendations for improving daily symptom management.


## Available Tools (4)
- **analyze_effectiveness**: Correlates subjective effectiveness and side effects with pharmacokinetic profile
- **get_medication_coverage**: Calculates predicted therapeutic windows and identifies coverage gaps
- **log_medication_event**: Records a specific instance of medication administration
- **suggest_optimization**: Provides data-driven suggestions to improve symptom management


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ADHD Medication Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just took 20mg of Adderall immediate release at 8:00 AM today. Can you log this for me?"

**🤖 AI Agent:**
> I have logged your 20mg dose of Adderall (immediate release) for 8:00 AM today.

---

**👤 You:**
> "How well has my Concerta been working over the last 7 days?"

**🤖 AI Agent:**
> Over the last 7 days, your Concerta has shown an average effectiveness rating of 7/10, with peak effectiveness typically occurring 4 hours after administration.

---

**👤 You:**
> "Show me my medication coverage for the last 24 hours."

**🤖 AI Agent:**
> In the last 24 hours, you had 10 hours of therapeutic coverage with a 3-hour gap identified in the late afternoon.


## ❓ FAQ

**Q: How do I record a new dose?**
You can use the `log_medication_event` tool to record the medication name, formulation type (immediate or extended), dosage in mg, and the exact timestamp.

**Q: What are coverage gaps?**
Coverage gaps are periods during the day when the medication concentration falls below the therapeutic threshold, which can be identified using `get_medication_coverage`.

**Q: Can this help me optimize my medication schedule?**
Yes, by using `suggest_optimization`, the system analyzes your logged data and coverage gaps to provide suggestions for adjusting timing or dosage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/adhd-medication-tracker](https://vinkius.com/en/ai-agent-connect/adhd-medication-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ADHD Medication Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adhd-medication-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ADHD Medication Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adhd-medication-tracker": {
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

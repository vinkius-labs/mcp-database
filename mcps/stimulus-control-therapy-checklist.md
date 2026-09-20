# Stimulus Control Therapy Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/stimulus-control-therapy-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generate personalized CBT-I stimulus control protocols and track sleep compliance.

## Description
This MCP server provides a specialized therapeutic bridge for implementing Stimulus Control Therapy (SCT), a core component of CBT-I. It helps users re-establish the association between the bed and sleep by generating customized rules, tracking protocol adherence, and analyzing sleep patterns. Use `generate_personalized_rules` to create a tailored protocol based on current bedroom habits, `calculate_compliance_score` to monitor adherence, `track_violations` to identify problematic nighttime behaviors, and `predict_habit_formation_timeline` to estimate when sleep stability will be achieved.


## Available Tools (4)
- **calculate_compliance_score**: Evaluates how well a user adhered to their stimulus control protocol over a specific period
- **generate_personalized_rules**: Creates a customized set of stimulus control instructions based on a user's current lifestyle and sleep issues
- **predict_habit_formation_timeline**: Projects when the user can expect the bed-sleep association to stabilize based on current adherence
- **track_violations**: Categorizes and analyzes specific breaches of the stimulus control protocol to identify patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stimulus Control Therapy Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have trouble falling asleep and I often use my laptop in bed. My wake time is 7:00 AM, I don't nap, and I usually go to bed around 11:00 PM. Can you make me a plan?"

**🤖 AI Agent:**
> Your personalized stimulus control protocol is ready. You must stop using your laptop in the bedroom. You must also leave the bed if you are not sleepy within 20 minutes. Always wake up at 7:00 AM to maintain sleep pressure.

---

**👤 You:**
> "I've been following my rules for 5 days. I followed my wake time every day, but I stayed in bed while awake once. What is my compliance score?"

**🤖 AI Agent:**
> Your current compliance score is 80%, which is categorized as 'Improving'.

---

**👤 You:**
> "Based on my current 85% compliance and the fact that my adherence is increasing, when will my sleep stabilize?"

**🤖 AI Agent:**
> You can expect sleep stability in approximately 3 weeks.


## ❓ FAQ

**Q: How do I create my personalized sleep rules?**
You can use the `generate_personalized_rules` tool by providing your current sleep difficulties, activities you do in bed, and your current wake-up time.

**Q: How can I track if I am following my protocol correctly?**
Use the `calculate_compliance_score` tool with your daily logs to receive a percentage score and status indicating your adherence level.

**Q: Can this tool help me identify why I am staying awake in bed?**
Yes, the `track_violations` tool analyzes your logs to identify frequent offender activities and assess your risk level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/stimulus-control-therapy-checklist](https://vinkius.com/en/ai-agent-connect/stimulus-control-therapy-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stimulus Control Therapy Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stimulus-control-therapy-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stimulus Control Therapy Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stimulus-control-therapy-checklist": {
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

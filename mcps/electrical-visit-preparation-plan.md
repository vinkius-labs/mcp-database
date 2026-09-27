# Electrical Visit Preparation Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/electrical-visit-preparation-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Prepare professional service requests and logistical plans for electrical repairs.

## Description
This MCP server helps users prepare for professional electrical service visits by enforcing strict safety boundaries. It transforms raw observations into structured service requests using `get_service_request`, creates logistical access plans via `generate_access_plan`, and provides observation checklists with `compile_evidence_checklist`. It also generates quality control questions through `get_completion_verification` and helps match the right professional using `select_provider`.


## Available Tools (5)
- **compile_evidence_checklist**: Provides a list of specific things to gather or observe to assist the technician
- **generate_access_plan**: Creates a logistical guide to ensure the technician can reach the necessary hardware
- **get_completion_verification**: Generates a set of quality-control questions for after the work is finished
- **get_service_request**: Generates a professional summary for a licensed electrician
- **select_provider**: Identifies the best matching professional from the user's available options


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electrical Visit Preparation Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a flickering light in the kitchen and the living room. The panel is in the basement and it is unlocked."

**🤖 AI Agent:**
> I can help you prepare for this. I will generate a professional service request for the flickering lights in the kitchen and living room, and create an access plan for your basement panel.

---

**👤 You:**
> "The circuit breaker keeps tripping in the garage. The panel is behind some heavy boxes."

**🤖 AI Agent:**
> I will generate a service request for the garage circuit issue and an access plan that instructs you to clear the boxes so the technician can reach the panel.

---

**👤 You:**
> "What should I look for to help the electrician with my outlet issue?"

**🤖 AI Agent:**
> I will provide an evidence checklist. Please observe if there are any unusual smells, sounds, or visible discoloration around the outlet, but do not touch the device.


## ❓ FAQ

**Q: Can I use this to diagnose my own electrical issues?**
No. This tool follows a strict No-DIY safety boundary. It is designed only to help you prepare information for a licensed professional.

**Q: How does `get_service_request` help me?**
It converts your description of the problem and affected rooms into a professional summary that a licensed electrician can use for accurate quoting.

**Q: What is an access plan?**
The `generate_access_plan` tool creates a guide to ensure the technician can reach your electrical panel and work safely without unnecessary interruptions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/electrical-visit-preparation-plan](https://vinkius.com/en/ai-agent-connect/electrical-visit-preparation-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electrical Visit Preparation Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electrical-visit-preparation-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electrical Visit Preparation Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electrical-visit-preparation-plan": {
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

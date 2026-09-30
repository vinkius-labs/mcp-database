# Device Disposal Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/device-disposal-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate secure decommissioning workflows and track device disposal tasks.

## Description
This MCP server provides specialized tools for managing the lifecycle of device decommissioning. It helps users ensure data security and environmental compliance by generating comprehensive checklists, evaluating sanitization readiness, and scheduling handoff tasks. Use `generate_disposal_checklist` to identify missing security steps, `validate_sanitization_readiness` to confirm if a device is safe for third-party handover, and `get_handoff_schedule` to manage timelines around a scheduled recycle date.


## Available Tools (4)
- **get_handoff_schedule**: Generates a timeline of tasks that must be performed to finalize the disposal process, centered around the recycling date
- **generate_disposal_checklist**: Creates a complete checklist of required actions based on device characteristics and identifies which security steps are still pending
- **query_device_requirements**: Retrieves the specific security requirements and mandatory steps for a given device type and disposal method
- **validate_sanitization_readiness**: Evaluates if the device is safe to be handed over to a third party based on the current security status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Device Disposal Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a disposal checklist for a Laptop with an SSD that hasn't been encrypted yet, and I haven't signed out of my accounts."

**🤖 AI Agent:**
> Your checklist is ready. You must complete the following steps: Sign out of all user accounts, enable full disk encryption, and perform a factory reset before proceeding with the disposal.

---

**👤 You:**
> "Is my smartphone safe to hand over for resale if I have backed up my data and signed out of my Google account, but encryption is disabled?"

**🤖 AI Agent:**
> The device is not yet safe for resale. Because encryption is disabled, there is a high risk of data exposure. It is recommended to enable encryption or perform a secure wipe before handing it over.

---

**👤 You:**
> "What is the schedule for a device being recycled on 2025-05-20?"

**🤖 AI Agent:**
> Your scheduled tasks are: Verify physical cleaning (Due: 2025-05-18), Prepare transport container (Due: 2025-05-19), and Hand over to recycler (Due: 2025-05-20).


## ❓ FAQ

**Q: How do I know if my device is safe to dispose of?**
You can use the `validate_sanitization_readiness` tool to evaluate if your device meets the necessary security requirements based on your backup, account sign-out, and encryption status.

**Q: Can I schedule tasks for my recycling date?**
Yes, the `get_handoff_schedule` tool generates a timeline of tasks centered around your specified recycle date to ensure a smooth handoff.

**Q: What information do I need for the checklist?**
To use `generate_disposal_checklist`, you will need to provide the device type, storage media type, backup status, account sign-out status, encryption status, and the intended disposal method.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/device-disposal-checklist](https://vinkius.com/en/ai-agent-connect/device-disposal-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Device Disposal Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `device-disposal-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Device Disposal Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "device-disposal-checklist": {
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

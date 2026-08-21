# Singapore MRT Delay Compensation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singapore-mrt-delay-compensation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Determine eligibility for MRT delay compensation based on official transit rules.

## Description
This MCP server provides deterministic tools to calculate compensation eligibility for passengers affected by Singapore MRT service disruptions. Using official transit guidelines, you can use `calculate_compensation_eligibility` to find out which transit pass you are entitled to based on the delay duration. You can also use `validate_line_identifier` to check if a specific line is supported, or `get_claim_window_status` to see if you are still within the 72-hour claim window.


## Available Tools (3)
- **validate_line_identifier**: Checks if a line name is valid
- **calculate_compensation_eligibility**: Determines MRT compensation eligibility
- **get_claim_window_status**: Checks if a claim is still eligible based on elapsed time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singapore MRT Delay Compensation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I was delayed by 45 minutes on the North South Line (NS). Am I eligible for compensation?"

**🤖 AI Agent:**
> Yes, you are eligible for a 2-day pass because your delay was between 30 and 59 minutes.

---

**👤 You:**
> "Is the Circle Line (CC) supported by this calculator?"

**🤖 AI Agent:**
> Yes, the Circle Line (CC) is a supported MRT line.

---

**👤 You:**
> "It has been 80 hours since my 120-minute delay on the East West Line (EW). Can I still claim?"

**🤖 AI Agent:**
> No, you are no longer eligible to file a claim as the 72-hour window has expired.


## ❓ FAQ

**Q: How do I know if I am eligible for compensation?**
You can use the `calculate_compensation_eligibility` tool. If your delay is 15 minutes or more, you will be eligible for a specific transit pass tier.

**Q: What is the deadline to file a claim?**
Claims must be submitted within 72 hours of the delay. You can verify your status using `get_claim_window_status`.

**Q: What proof do I need to provide?**
Standard claims require a Delay Certificate or EZ-Link tap-in/out data for digital verification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singapore-mrt-delay-compensation-calculator](https://vinkius.com/ai-agent-connect/singapore-mrt-delay-compensation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singapore MRT Delay Compensation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singapore-mrt-delay-compensation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singapore MRT Delay Compensation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singapore-mrt-delay-compensation-calculator": {
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

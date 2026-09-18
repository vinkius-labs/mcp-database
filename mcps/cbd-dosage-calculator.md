# CBD Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cbd-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Personalized CBD dosage plans and titration schedules based on wellness goals.

## Description
This MCP server provides precise, research-based CBD dosage recommendations. By using tools like `calculate_dosage_plan`, users can receive a complete regimen including starting doses, titration steps, and optimal timing for goals such as sleep, anxiety, pain, or recovery. It also includes `get_goal_thresholds` to understand therapeutic ranges and `validate_product_suitability` to ensure product concentrations are practical for the intended dose.


## Available Tools (4)
- **calculate_dosage_plan**: Provides a complete, personalized CBD regimen including starting dose, titration steps, and timing
- **get_goal_thresholds**: Informs the user about the typical therapeutic milligram ranges for their specific wellness goal
- **get_timing_guidance**: Explains why a specific administration time is recommended for a given goal
- **validate_product_suitability**: Determines if a specific product concentration is practical for the user's calculated dose


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CBD Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 70kg and I am new to CBD. I want to use it for sleep. What is my dosage plan?"

**🤖 AI Agent:**
> Your starting dose is 15mg. You should take this in the evening. Your titration schedule involves staying at 15mg for 5 days, then increasing to 30mg for 5 days.

---

**👤 You:**
> "What is the typical therapeutic range for anxiety?"

**🤖 AI Agent:**
> For anxiety, the typical therapeutic range is between 25mg and 75mg per day.

---

**👤 You:**
> "Is it a good idea to take my CBD in the morning for sleep?"

**🤖 AI Agent:**
> No, for sleep goals, it is better to take the dose in the evening or at night to align with your circadian rhythm.


## ❓ FAQ

**Q: How does the dosage calculation work?**
The `calculate_dosage_plan` tool uses your body weight, experience level, and specific wellness goal to determine a safe starting dose and a gradual titration schedule.

**Q: Can I check if my CBD product is suitable for my dose?**
Yes, you can use the `validate_product_suitability` tool to check if the concentration of your product allows for an accurate and practical dose.

**Q: What wellness goals are supported?**
The server supports dosage planning for sleep, anxiety, pain, and recovery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cbd-dosage-calculator](https://vinkius.com/en/ai-agent-connect/cbd-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CBD Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cbd-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CBD Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cbd-dosage-calculator": {
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

# Calories Burned Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calories-burned-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate calories burned using MET values and heart rate data.

## Description
This MCP server provides a comprehensive way to estimate energy expenditure. Use `list_activities` to find MET values for various exercises, and `calulate_met_burn` to compute calories based on weight and duration. For more complex scenarios, `calculate_hr_burn` uses heart rate data via Keyence or BMI-based methods. You can also use `get_food_equivalence` to see how much food you'd need to eat to match your burn.


## Available Tools (4)
- **calculate_hr_burn**: Calculate calories burned based on heart rate
- **calculate_met_burn**: Calculate calories burned based on MET value and duration
- **get_food_equivalence**: Find food equivalents for a specific calorie amount
- **list_activities**: List available physical activities and their MET values


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calories Burned Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories did I burn running for 30 minutes at a moderate intensity if I weigh 70kg?"

**🤖 AI Agent:**
> You burned approximately 250 calories.

---

**👤 You:**
> "What is a good activity for high intensity?"

**🤖 AI Agent:**
> Running at a vigorous level has a high MET value and will burn significant calories.

---

**👤 You:**
> "How much pizza is 500 calories worth?"

**🤖 AI Agent:**
> 500 calories is roughly equivalent to 2 slices of pepperoni pizza.


## ❓ FAQ

**Q: How accurate are the calculations?**
The accuracy depends on the precision of your inputs, such as body weight and heart rate. The `calculate_met_burn` tool uses standard MET values from the Compendium of Physical Activities.

**Q: Can I use my own heart rate data?**
Yes, the `calculate_hr_burn` tool allows you to estimate burn using measured heart rate and age via Keyence or BMI-based methods.

**Q: What is a MET value?**
A Metabolic Equivalent of Task (MET) represents the energy cost of an activity. One MET is the energy used while sitting at rest.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calories-burned-calculator](https://vinkius.com/mcp/calories-burned-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calories Burned Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calories-burned-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calories Burned Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calories-burned-calculator": {
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

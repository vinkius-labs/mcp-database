# Sick-Day Insulin Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sick-day-insulin-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates insulin adjustments, monitoring frequency, and hydration needs during illness.

## Description
This MCP server provides deterministic calculations to manage insulin-dependent diabetes during illness. It uses physiological markers like body temperature, blood glucose, and ketone levels to determine necessary adjustments. Use `calculate_sick_day_adjustments` to get a full profile of insulin increases, monitoring intervals, and hydration targets. You can also use `get_ketone_severity_guidance` for medical urgency instructions and `check_hydration_status` to track fluid intake against increased sick-day requirements.


## Available Tools (3)
- **get_ketone_severity_guidance**: Provides specific medical urgency instructions based solely on ketone presence
- **calculate_sick_day_adjustments**: Provides a comprehensive set of adjustments for insulin, monitoring, and hydration based on current physiological markers
- **check_hydration_status**: Validates if the user's current fluid intake is sufficient to meet the increased sick-day requirement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sick-Day Insulin Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a fever of 38.5°C, my blood glucose is 180 mg/dL, and I have small ketones. My baseline insulin is 40 units. What are my adjustments?"

**🤖 AI Agent:**
> Your fever increases insulin needs by 10%. Including the illness stress factor, your total insulin requirement is increased. You should check your glucose every 2-4 hours and aim for 60ml of hydration based on your baseline. Since ketones are small, continue routine monitoring.

---

**👤 You:**
> "I'm feeling very sick with a temperature of 39°C and moderate ketones. My baseline insulin is 30 units."

**🤖 AI Agent:**
> Warning: Moderate ketones detected. You should seek medical advice immediately. Your insulin requirements are increased due to the 39°C fever and illness stress. Ensure you follow the increased hydration targets.

---

**👤 You:**
> "I've drunk 1000ml of water today. My baseline insulin is 40 units. Have I met my sick-day hydration goal?"

**🤖 AI Agent:**
> No, you have not met your target. Based on your baseline, you need 60ml more to reach your sick-day hydration requirement.


## ❓ FAQ

**Q: How does fever affect my insulin needs?**
If your temperature is above 37.5°C, the `calculate_sick_day_adjustments` tool increases the insulin requirement by 10% for every degree above that threshold.

**Q: What should I do if I detect ketones?**
You should use `get_ketone_severity_guidance` to determine the level of medical urgency. Moderate or large ketone levels require immediate medical consultation.

**Q: How much water should I drink when sick?**
The tool calculates a hydration target that is 50% higher than your baseline needs. You can use `check_hydration_status` to see if you have met this target.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sick-day-insulin-adjuster](https://vinkius.com/ai-agent-connect/sick-day-insulin-adjuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sick-Day Insulin Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sick-day-insulin-adjuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sick-Day Insulin Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sick-day-insulin-adjuster": {
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

# Body Fat Percentage Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/body-fat-percentage-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate body fat, lean mass, and fat mass using the US Navy method.

## Description
This MCP server provides precise body composition analysis using the standardized US Navy circumference method. It allows AI agents to calculate body fat percentage, fat mass, and lean mass based on anthropometric measurements like height, neck, waist, and hip circumferences. Use `estimate_body_composition` for a full profile or `get_composition_summary` to translate percentages into weight-based metrics. It also includes `validate_anthropometric_measurements` to ensure input data falls within realistic biological ranges.


## Available Tools (4)
- **get_composition_summary**: Provides a simplified, human-readable summary of the user's body composition
- **get_fitness_category_bounds**: Provides the numerical ranges for the various fitness categories
- **estimate_body_composition**: For females, hip circumference is required.

Calculates the full body composition profile including fat percentage, fat mass, and lean mass using the US Navy method
- **validate_anthropometric_measurements**: Checks if the provided measurements are within realistic human biological ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Body Fat Percentage Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my body composition. I am a male, 85kg, 180cm tall, with a 40cm neck and 90cm waist."

**🤖 AI Agent:**
> Your body fat percentage is 18.5%. Your fat mass is 15.7kg and your lean mass is 69.3kg. Your fitness category is 'Fitness'.

---

**👤 You:**
> "What is the body composition summary for a 20% body fat and 70kg weight?"

**🤖 AI Agent:**
> With 20% body fat at 70kg, your fat mass is 14kg and your lean mass is 56kg.

---

**👤 You:**
> "I am a female, 60kg, 165cm tall, 32cm neck, 70cm waist, and 95cm hips. What is my body fat?"

**🤖 AI Agent:**
> Your body fat percentage is 28%. Your fat mass is 16.8kg and your lean mass is 43.2kg. Your fitness category is 'Acceptable'.


## ❓ FAQ

**Q: How accurate is the US Navy method?**
The US Navy method is a widely recognized anthropometric formula that provides a reliable estimate of body fat percentage based on circumference measurements.

**Q: What measurements are required for women?**
For female users, the `estimate_body_composition` tool requires height, weight, neck circumference, waist circumference, and hip circumference to ensure biological accuracy.

**Q: Can I validate my measurements before calculating?**
Yes, you can use the `validate_anthropometric_measurements` tool to check if your provided dimensions are within realistic human biological ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/body-fat-percentage-estimator](https://vinkius.com/en/ai-agent-connect/body-fat-percentage-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Body Fat Percentage Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `body-fat-percentage-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Body Fat Percentage Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "body-fat-percentage-estimator": {
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

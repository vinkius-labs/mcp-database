# Deadlift Setup Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/deadlift-setup-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Calculate optimal deadlift setup parameters like hip height and stance width based on your body measurements.

## Description
This MCP server provides precise anthropometric calculations to optimize deadlift performance. By inputting your height, arm length, torso length, and leg length, you can determine the most efficient setup for your specific build. Use `get_setup_parameters` to find your ideal hip height, stance width, and grip width. You can also use `get_mechanical_advantage_profile` to understand your leverage type, or `compare_variations` to decide between conventional and sumo styles. Finally, use `validate_setup_readiness` to ensure your calculated position is mechanically safe.


## Available Tools (4)
- **compare_variations**: Compares the calculated setup for Conventional vs. Sumo for a specific individual
- **get_mechanical_advantage_profile**: Provides a qualitative assessment of how the lifter's proportions affect their deadlift efficiency
- **get_setup_parameters**: Calculates specific physical setup dimensions based on user body measurements
- **validate_setup_readiness**: Checks if the calculated setup parameters are within safe physiological bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deadlift Setup Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my deadlift setup for a conventional style. I am 180cm tall, have 80cm arms, 55cm torso, and 90cm legs."

**🤖 AI Agent:**
> Your optimal conventional setup includes a hip height of 42.5cm, a stance width of 25.0cm, and a grip width of 52.0cm with a Neutral spine angle.

---

**👤 You:**
> "Should I do sumo or conventional? I have 85cm arms, 50cm torso, and 95cm legs, and I am 175cm tall."

**🤖 AI Agent:**
> Based on your proportions, the Sumo variation is optimal, offering a 5.2cm reduction in range of motion compared to conventional.

---

**👤 You:**
> "What is my mechanical advantage profile with 75cm arms, 60cm torso, and 85cm legs?"

**🤖 AI Agent:**
> You have a Standard-Lever profile, with Hip Drive being your primary limiting factor.


## ❓ FAQ

**Q: How accurate are these setup calculations?**
The calculations are based on established deadlift anthropometric guidelines and the specific limb measurements you provide.

**Q: Can I use this for both conventional and sumo deadlifts?**
Yes, you can use `get_setup_parameters` for both styles by specifying the variation in the tool input.

**Q: What is a mechanical advantage profile?**
It is a classification of your body proportions, such as Long-Lever or Short-Lever, which helps identify how your limb lengths affect your lifting efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/deadlift-setup-calculator](https://vinkius.com/en/ai-agent-connect/deadlift-setup-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deadlift Setup Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deadlift-setup-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deadlift Setup Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deadlift-setup-calculator": {
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

# Digital Wellness Boundary Setter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/digital-wellness-boundary-setter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Establish healthy digital habits with personalized notification schedules, social media limits, and a digital sunset time.

## Description
The Digital Wellness Boundary Setter helps you reclaim your attention by calculating optimal digital boundaries. Using the `calculate_boundaries` tool, you can generate a personalized plan including focus blocks and social media limits based on your work intensity and entertainment preferences. The `analyze_usage_gap` tool identifies exactly where time is being lost by comparing current app usage to your desired targets. Additionally, use `predict_wellbeing_uplift` to estimate how much your mental clarity and stress levels might improve if you adhere to these new boundaries.


## Available Tools (3)
- **analyze_usage_gap**: Compares current digital habits against desired limits
- **calculate_boundaries**: Generates a personalized digital boundary plan
- **predict_wellbeing_uplift**: Estimates the potential increase in a user's well-being score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Wellness Boundary Setter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a high work intensity and prefer low entertainment. What should my digital boundaries look like?"

**🤖 AI Agent:**
> Your plan includes deep focus blocks from 09:00 to 12:00 and 14:00 to 17:00. Your digital sunset is set for 21:30, and your daily limit for social media platforms like Instagram is 30 minutes.

---

**👤 You:**
> "Analyze this usage data: [{'appName': 'TikTok', 'currentMinutes': 120, 'desiredMinutes': 30}, {'appName': 'Instagram', 'currentMinutes': 60, 'desiredMinutes': 20}]"

**🤖 AI Agent:**
> You can reclaim a total of 130 minutes. TikTok shows a discrepancy of 90 minutes, and Instagram shows a discrepancy of 40 minutes.

---

**👤 You:**
> "If my stress level is 8 and I am 70% sure I can stick to the plan, what is my predicted well-being improvement?"

**🤖 AI Agent:**
> Your predicted well-being score improvement is +1.2, with a high confidence interval.


## ❓ FAQ

**Q: How does the boundary calculation work?**
The `calculate_boundaries` tool uses your work intensity and entertainment preferences to determine when you should focus and when you can engage with social media, including a designated digital sunset time.

**Q: Can I see how much time I can reclaim?**
Yes, by using the `analyze_usage_gap` tool with your current app usage data, you can identify specific platforms where you are over-limit and see the total minutes you could reclaim.

**Q: How is well-being improvement estimated?**
The `predict_wellbeing_uplift` tool calculates an estimated score improvement by analyzing your current stress level and how likely you are to stick to the new boundaries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/digital-wellness-boundary-setter](https://vinkius.com/mcp/digital-wellness-boundary-setter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Wellness Boundary Setter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-wellness-boundary-setter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Wellness Boundary Setter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-wellness-boundary-setter": {
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

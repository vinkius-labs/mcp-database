# Crowdfunding Pitch Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdfunding-pitch-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze crowdfunding campaign effectiveness using linguistic analysis of narrative ratio, rewards, and trust.

## Description
The Crowdfunding Pitch Scorer evaluates your campaign text for key success factors. Use `narrative_ratio_tool` to check the balance between storytelling and the funding request, and `reward_token_tool` to ensure your rewards are distinct. The `persuasion_elements_tool` quantifies scarcity and social proof triggers, while `transparency_audit_tool` audits for risk disclosures and timeline clarity.

### Available Tools

`score_narrative_ratio`, `check_reward_tiers`, `count_persuasion_elements`, `audit_transparency`


## Available Tools (4)
- **score_narrative_ratio**: Analyzes the ratio of storytelling to the funding request
- **count_persuasion_elements**: Quantifies scarcity and social proof elements
- **check_reward_tiers**: Evaluates the clarity and differentiation of reward tiers
- **audit_transparency**: Audits for risk disclosures and timeline information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crowdfunding Pitch Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this pitch for narrative balance: 'Our project is amazing because we love making toys. Please back us with $5000.'"

**🤖 AI Agent:**
> The narrative ratio is 0.2, indicating an extremely high ask-to-story ratio.

---

**👤 You:**
> "Check if my rewards are clear: 'Tier 1: Sticker. Tier 2: T-shirt. Tier 3: Hoodie.'"

**🤖 AI Agent:**
> Your reward tiers have a differentiation score of 90/100.

---

**👤 You:**
> "Are there scarcity triggers in this text? 'Only 50 units left! We were featured in TechCrunch!'"

**🤖 AI Agent:**
> Found 1 scarcity trigger and 1 social proof mention.


## ❓ FAQ

**Q: How does the tool evaluate narrative balance?**
It uses `narrative_ratio_tool` to compare storytelling text against funding request keywords. Tools available: `score_narrative_ratio`, `check_reward_tiers`, `count_persuasion_elements`.

**Q: Can I check for social proof?**
Yes, the `persuasion_elements_tool` identifies mentions of press, backers, and prior successes.

**Q: Does it help with reward clarity?**
Yes, use `reward_tier_tool` to assess how well your tiers are differentiated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdfunding-pitch-scorer](https://vinkius.com/mcp/crowdfunding-pitch-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crowdfunding Pitch Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crowdfunding-pitch-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crowdfunding Pitch Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crowdfunding-pitch-scorer": {
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

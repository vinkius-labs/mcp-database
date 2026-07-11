# Referral Program Copy Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/referral-program-copy-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze referral program marketing copy for clarity, friction, and effectiveness.

## Description
The Referral Program Copy Scorer is an analytical tool designed to evaluate the effectiveness of your referral marketing materials. It helps you minimize cognitive load and maximize user participation by auditing key elements of your copy. Using tools like `score_incentive_clarity`, you can ensure both referrers and referees understand their rewards. The `calculate_friction_score` identifies complex instructions that might cause drop-offs, while `audit_cta_specificity` ensures your buttons are actionable. Additionally, `check_compliance_visibility` verifies legal transparency, and `identify_reward_framing` analyzes how value is communicated (e.g., currency vs percentage). This MCP connects your AI agents to deep marketing analytics for high-conversion referral programs.


## Available Tools (5)
- **identify_reward_framing**: Identifies which psychological method is being used to communicate value
- **score_incentive_clarity**: Determines if both the sender and the receiver benefits are clearly articulated in the text
- **audit_cta_specificity**: Assesses if the call-to-action provides enough detail for a user to act without confusion
- **calculate_friction_score**: Evaluates how much cognitive effort is required based on the length and complexity of the instructions
- **check_compliance_visibility**: Verifies that legal disclaimers or links to terms are present to ensure transparency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Referral Program Copy Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this referral text: 'Invite a friend and you both get $10! Click here to start sharing. Terms apply.'"

**🤖 AI Agent:**
> The incentive clarity is high as both parties are mentioned. The reward framing is CURRENCY ($10). The CTA specificity is moderate, and compliance visibility is confirmed by the presence of 'Terms apply'.

---

**👤 You:**
> "Check the friction level for these instructions: 'Go to your settings, click on the referral tab, copy your unique link, and paste it into a message to your best friend.'"

**🤖 AI Agent:**
> The friction level is High due to the multiple steps required in the instruction text.

---

**👤 You:**
> "Is this CTA effective: 'Get 20% off your next order by using our referral link!'"

**🤖 AI Agent:**
> The reward framing is PERCENTAGE (20%). The CTA is actionable, though adding specific action steps could improve the specificity rating.


## ❓ FAQ

**Q: How does the tool measure incentive clarity?**
The `score_incentive_clarity` tool checks if the rewards for all expected parties, such as both the sender and receiver, are explicitly stated in your text.

**Q: Can I analyze different types of reward presentations?**
Yes, the `identify_reward_framing` tool can detect if rewards are presented as currency, percentages, or platform credits.

**Q: How is sharing friction calculated?**
The `calculate_friction_score` tool evaluates the word count and complexity of your instructions to determine if the effort required is Low, Medium, or High.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/referral-program-copy-scorer](https://vinkius.com/mcp/referral-program-copy-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Referral Program Copy Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `referral-program-copy-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Referral Program Copy Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "referral-program-copy-scorer": {
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

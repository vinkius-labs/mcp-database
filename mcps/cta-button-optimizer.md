# CTA Button Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cta-button-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [copywriting](../categories/copywriting.md)

Analyze the psychological impact, verb strength, and visual fit of your Call-to-Action (CTA) copy.

## Description
The CTA Button Optimizer is a specialized tool for copywriters and UX designers to evaluate the effectiveness of button and link text. By using `analyze_copy_strength`, you can assess verb impact, linguistic framing (first vs second person), and identify friction or urgency markers that influence conversion rates. Additionally, use `check_dimension_fit` to ensure your CTA remains legible across all devices by checking character counts against mobile and desktop constraints. This tool helps prevent cognitive dissonance between headlines and actions, ensuring a high-performing user experience.


## Available Tools (2)
- **analyze_copy_strength**: Analyzes the psychological impact and strength of a CTA string
- **check_dimension_fit**: Checks if CTA text fits within device-specific character limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CTA Button Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this CTA: 'Claim your free trial today!'"

**🤖 AI Agent:**
> Verb Strength Score: 0.85. Framing: second_person. Friction Word Count: 1 ('free'). Urgency Score: 0.9 (detected 'today').

---

**👤 You:**
> "Is the text 'Get my discount' suitable for a mobile button?"

**🤖 AI Agent:**
> is_fit: true. current_character_count: 15. overflow_risk: low.

---

**👤 You:**
> "Evaluate the strength of 'Click here to submit'."

**🤖 AI Agent:**
> Verb Strength Score: 0.15. Framing: second_person. Friction Word Count: 0. Urgency Score: 0.0.


## ❓ FAQ

**Q: How does the tool evaluate verb strength?**
The `analyze_copy_strength` tool compares your text against a lexicon of impactful verbs (like 'Claim' or 'Unlock') and generic verbs (like 'Click' or 'Submit') to provide a strength score.

**Q: Can I check if my CTA is too long for mobile screens?**
Yes, by using the `check_dimension_fit` tool and specifying 'mobile' as the device type, you can detect if your text exceeds character limits that might cause overflow.

**Q: Does this tool identify friction words?**
Yes, the analysis identifies phrases like 'free' or 'no credit card' and provides a count of these low-barrier markers to help you balance urgency with quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cta-button-optimizer](https://vinkius.com/mcp/cta-button-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CTA Button Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cta-button-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CTA Button Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cta-button-optimizer": {
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

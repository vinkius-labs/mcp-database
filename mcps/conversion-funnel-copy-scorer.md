# Conversion Funnel Copy Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conversion-funnel-copy-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze marketing funnel stages for message match, friction words, and CTA alignment.

## Description
The Conversion Funnel Copy Scorer is an analytical utility designed to measure linguistic and strategic alignment throughout a marketing funnel. By comparing text from different stages--such as ads, landing pages, and checkout screens--it identifies critical drop-off risks. The tool uses `calculate_copy_score` to evaluate keyword overlap and semantic consistency between consecutive stages. It also quantifies friction intensity by detecting high-resistance words like 'required' or 'must' and suggests low-friction alternatives like 'explore'. Additionally, it detects reading level drift to prevent cognitive overload and assesses CTA alignment to ensure the promise made in your ads is fulfilled at checkout.


## Available Tools (1)
- **calculate_copy_score**: Calculate similarity between two pieces of text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conversion Funnel Copy Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the text from my Facebook ad: 'Get 50% off today!' with my landing page: 'Claim your 50% discount now.'"

**🤖 AI Agent:**
> The keyword overlap score is high due to the shared '50%' and 'discount/off' concepts, maintaining strong message match.

---

**👤 You:**
> "Check if my checkout page has too much friction compared to the landing page."

**🤖 AI Agent:**
> The analysis detected 3 high-friction words ('required', 'submit', 'must') on the checkout page that were not present in the landing page.

---

**👤 You:**
> "Evaluate the reading level consistency between my ad and my product description."

**🤖 AI Agent:**
> A significant reading level delta was detected, indicating a jump in complexity that might cause user drop-off.


## ❓ FAQ

**Q: How does the tool measure message match?**
It uses `calculate_copy_score` to analyze keyword overlap and semantic consistency between two provided text segments from different funnel stages.

**Q: Can it identify words that cause users to drop off?**
Yes, the tool scans for high-friction words like 'must' or 'pay' and suggests softer alternatives to reduce psychological resistance.

**Q: What stages of the funnel can be analyzed?**
The tool is optimized for analyzing transitions between common stages like ads, landing pages, and checkout screens.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conversion-funnel-copy-scorer](https://vinkius.com/mcp/conversion-funnel-copy-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conversion Funnel Copy Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `conversion-funnel-copy-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conversion Funnel Copy Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conversion-funnel-copy-scorer": {
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

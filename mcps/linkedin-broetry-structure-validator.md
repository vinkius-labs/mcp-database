# LinkedIn Broetry Structure Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-broetry-structure-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Analyze LinkedIn posts for adherence to the 'broetry' writing style using structural metrics.

## Description
The LinkedIn Broetry Structure Validator evaluates how well a post follows the high-engagement 'broetry' format. By analyzing text patterns, it calculates key metrics like single-sentence paragraph ratios, whitespace density, and orphan-line detection. Use `analyze_post_structure` to get raw structural data, `detect_formatting_deviations` to find traditional multi-sentence blocks, and `evaluate_style_adherence` to receive a qualitative score of the post's stylistic adherence.


## Available Tools (3)
- **analyze_post_structure**: Analyze the structural metrics of a LinkedIn post
- **detect_formatting_deviations**: g., multiple sentences in one paragraph).

Detect formatting deviations in a LinkedIn post
- **evaluate_style_adherence**: Evaluate how well a post adheres to the LinkedIn Broetry style


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Broetry Structure Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this LinkedIn post: 'Success is not final.\n\nFailure is not fatal.\n\nIt is the courage to continue that counts.'"

**🤖 AI Agent:**
> The structural analysis shows a high single-sentence paragraph ratio and optimal whitespace density, indicating strong adherence to the broetry style.

---

**👤 You:**
> "Check for formatting deviations in this text: 'This is a long paragraph. It contains multiple sentences that break the rhythm of broetry.'"

**🤖 AI Agent:**
> One deviation was detected at line 1, where a multi-sentence block violates the single-sentence paragraph rule.

---

**👤 You:**
> "Evaluate style adherence for a post with a 0.9 ratio, 1 deviation, and 0.2 whitespace ratio."

**🤖 AI Agent:**
> The post falls into the 'Mixed Style' category with an adherence score of 85.0.


## ❓ FAQ

**Q: What is 'broetry'?**
'Broetry' refers to a specific LinkedIn writing style characterized by short, punchy sentences and significant use of whitespace to drive engagement through vertical scrolling.

**Q: How does the tool detect deviations?**
The `detect_formatting_deviations` tool scans for paragraphs containing three or more sentences, which indicates a departure from the single-sentence paragraph standard of broetry.

**Q: Can I use this for any text?**
While it works on any text, the metrics and adherence scores are specifically optimized for analyzing LinkedIn post structures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-broetry-structure-validator](https://vinkius.com/mcp/linkedin-broetry-structure-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Broetry Structure Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-broetry-structure-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Broetry Structure Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-broetry-structure-validator": {
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

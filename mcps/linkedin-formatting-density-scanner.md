# LinkedIn Formatting Density Scanner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-formatting-density-scanner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Analyze LinkedIn post visual structure, whitespace ratio, and mobile scannability.

## Description
The LinkedIn Formatting Density Scanner provides precision analytics for evaluating the visual rhythm of LinkedIn content. Using tools like `analyze_paragraph_distribution`, `evaluate_whitespace_ratio`, `detect_stylance_elements`, and `estimate_mobile_viewport_depth`, creators can quantify 'scannability'--the ability of a post to capture attention in a fast-scrolling feed. This MCP server calculates paragraph length distribution, identifies Unicode styling density, measures whitespace ratios, and estimates mobile viewport scroll depth based on exact character and line count mathematics.


## Available Tools (1)
- **analyze_paragraph_distribution**: Analyze the structural rhythm of a text by identifying single vs multi-sentence blocks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Formatting Density Scanner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the formatting density of this post: 'LinkedIn is changing. Every day I see new updates. It is hard to keep up.'"

**🤖 AI Agent:**
> Analysis complete. Single-sentence blocks: 3, Multi-sentence blocks: 0. The text follows a high-scannability pattern with frequent line breaks.

---

**👤 You:**
> "Check the whitespace ratio for this content: 'Line 1

Line 2
Line 3'"

**🤖 AI Agent:**
> The whitespace ratio is 0.5, indicating a high proportion of empty space relative to text lines.

---

**👤 You:**
> "Detect any stylistic elements in: '<0xF0><0x9D><0x91><0xA9>𝒐𝒍𝒅 𝑻𝒆𝒙𝒕 and 😊 emojis'"

**🤖 AI Agent:**
> Detected 10 Unicode styling characters and 1 emoji. The post contains high visual density elements.


## ❓ FAQ

**Q: What metrics does this tool analyze?**
The tool analyzes paragraph distribution (single vs multi-sentence blocks), whitespace ratio, Unicode styling density, emoji count, and estimated mobile scroll depth.

**Q: How is the whitespace ratio calculated?**
It compares the number of completely empty lines to the total count of all line breaks in your provided text.

**Q: Can I use this for posts other than LinkedIn?**
While optimized for LinkedIn's 'broetry' style, the structural analysis works on any text-based content where line breaks and paragraph spacing are significant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-formatting-density-scanner](https://vinkius.com/mcp/linkedin-formatting-density-scanner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Formatting Density Scanner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-formatting-density-scanner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Formatting Density Scanner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-formatting-density-scanner": {
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

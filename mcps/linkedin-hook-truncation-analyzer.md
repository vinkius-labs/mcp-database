# LinkedIn Hook Truncation Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-hook-truncation-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Analyze LinkedIn post hooks for visibility, truncation, and engagement potential.

## Description
Maximize your LinkedIn engagement by ensuring your content is visible before the 'See more' cutoff. This MCP server provides specialized tools to analyze post openings: `analyze_truncation_metrics` calculates character and pixel-width density for desktop and mobile; `identify_hook_classification` detects patterns like Question, Statistic, or Listicle hooks; and `evaluate_scroll_stopper_score` measures punctuation variance and rhythm to estimate engagement potential.


## Available Tools (3)
- **analyze_truncation_metrics**: Determines if the post's hook will be visible on specific devices and calculates formatting density
- **evaluate_scroll_stopper_score**: Calculates a numerical score representing the "scroll-stopping" and engagement potential of the hook
- **identify_hook_classification**: Analyzes the text to determine which of the five specific LinkedIn hook types are being as used


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Hook Truncation Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Will my LinkedIn post be truncated on mobile? Here is the text: 'Stop wasting time on manual outreach. It is killing your productivity and costing you thousands in lost revenue every single month.'"

**🤖 AI Agent:**
> The post exceeds the 150-character mobile limit. Visible text: 'Stop wasting time on manual outreach. It is killing your productivity and costing you thousands in lost...' (Truncated).

---

**👤 You:**
> "What type of hook am I using here: 'Did you know that 85% of LinkedIn users scroll past posts without reading the first line?'"

**🤖 AI Agent:**
> The tool identified this as a Statistic hook with high confidence due to the presence of numerical data (85%).

---

**👤 You:**
> "Analyze the engagement potential of this opening: 'I used to hate cold calling. Then I found a system that changed everything.'"

**🤖 AI Agent:**
> The scroll-stopper score is 78/100, driven by high punctuation variance and effective use of short sentence fragments.


## ❓ FAQ

**Q: How does the truncation analysis work?**
The `analyze_truncation_metrics` tool checks your text against LinkedIn's specific limits: approximately 210 characters for desktop and 150 characters for mobile, providing exact counts and estimated pixel width.

**Q: Can it identify different types of hooks?**
Yes, using `identify_hook_classification`, the tool detects if your post starts with a Question, Statistic, Listicle, Story Setup, or Contrarian hook based on structural patterns.

**Q: What is the scroll-stopper score?**
The `evaluate_scroll_stopper_score` tool calculates a score based on punctuation diversity and sentence fragment rhythm, helping you understand how effectively your hook interrupts the user's scroll.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-hook-truncation-analyzer](https://vinkius.com/mcp/linkedin-hook-truncation-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Hook Truncation Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-hook-truncation-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Hook Truncation Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-hook-truncation-analyzer": {
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

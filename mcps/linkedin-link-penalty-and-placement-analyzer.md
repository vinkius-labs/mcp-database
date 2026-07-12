# LinkedIn Link Penalty and Placement Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-link-penalty-and-placement-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyzes LinkedIn post text to identify external link placement risks and bypass phrase detection.

## Description
The LinkedIn Link Penalty and Placement Analyzer helps users assess the risk of algorithmic reach reduction by examining post content. It uses `analyze_url_placement` to find URLs and check if they are in the 'hook zone', `identify_workaround_signals` to detect bypass phrases, and `evaluate_risk_report` to generate a final risk score based on positioning and manipulation patterns.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Link Penalty and Placement Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this post for link placement: 'Check out https://marketing-pro.com for more info!'"

**🤖 AI Agent:**
> The URL https://marketing-pro.com was found at index 9, which is within the hook zone.

---

**👤 You:**
> "Are there any bypass signals in this text: 'I will put the link in the first comment below.'"

**🤖 AI Agent:**
> Detected bypass phrases: ['link in the first comment below'].

---

**👤 You:**
> "Calculate the risk report for a post with a link at index 50 and no bypass phrases."

**🤖 AI Agent:**
> The calculated risk score is 0, resulting in a LOW risk level.


## ❓ FAQ

**Q: What is the Hook Zone?**
The Hook Zone refers to the first 18 characters of a post. Links placed here are highly susceptible to visibility penalties. Tools available: `your_tool_name`.

**Q: How does it detect bypass phrases?**
The `identify_workaround_signals` tool scans for specific text patterns like 'link in comments' that suggest users are trying to circumvent the algorithm.

**Q: Can I use this for other social platforms?**
This tool is specifically optimized for LinkedIn's feed algorithm and its unique link placement penalties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-link-penalty-and-placement-analyzer](https://vinkius.com/mcp/linkedin-link-penalty-and-placement-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Link Penalty and Placement Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-link-penalty-and-placement-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Link Penalty and Placement Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-link-penalty-and-placement-analyzer": {
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

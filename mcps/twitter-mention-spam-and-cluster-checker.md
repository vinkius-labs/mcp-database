# Twitter Mention Spam and Cluster Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twitter-mention-spam-and-cluster-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detects @-mention clustering and structural spam patterns to prevent shadowbans.

## Description
This MCP server provides a suite of diagnostic tools for analyzing tweet structures. Use `evaluateTweetStructure` to identify pattern violations like excessive leading mentions, `calculateClusteringRisk` to detect high-density mention groups, `computeShadowbanScore` to assess overall risk based on mention-to-text ratios, and `validateHashtagMentionSpacing` to ensure proper separation between hashtags and mentions.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twitter Mention Spam and Cluster Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this tweet for spam patterns: '@user1 @user2 @user3 @user4 Hello world'"

**🤖 AI Agent:**
> A pattern violation was detected because the post starts with four or more consecutive mentions.

---

**👤 You:**
> "Are these mentions clustered? '@a @b @c'"

**🤖 AI Agent:**
> Yes, a cluster of 3 mentions was found within the character window.

---

**👤 You:**
> "Check the spacing between hashtags and mentions in '#news @breaking'"

**🤖 AI Agent:**
> The spacing is valid with a distance ratio of 6.


## ❓ FAQ

**Q: How can I check if my tweet is at risk of being flagged?**
You can use the `computeShadowbanScore` tool to analyze your text and see the calculated risk level. Tools available: `your_tool_name`.

**Q: What defines a mention cluster?**
The `calculateClusteringRisk` tool flags any instance where three or more @-mentions appear within a 20-character window.

**Q: Does it detect spam patterns at the start of a tweet?**
Yes, `evaluateTweetStructure` specifically checks if a post begins with four or more consecutive mentions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twitter-mention-spam-and-cluster-checker](https://vinkius.com/mcp/twitter-mention-spam-and-cluster-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twitter Mention Spam and Cluster Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twitter-mention-spam-and-cluster-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twitter Mention Spam and Cluster Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twitter-mention-spam-and-cluster-checker": {
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

# LinkedIn Mention and Tag Distribution Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-mention-and-tag-distribution-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Quantify the strategic placement of @mentions and #hashtags in LinkedIn posts.

## Description
This MCP server provides analytical capabilities for LinkedIn content optimization. Use `count_entities` to tally @mentions and #hashtasts, and `get_first_mention_distance` to find the lead-in text length. You can also use `analyze_tag_distribution` to measure symbol clustering and `verify_signature_placement` to check for signature block usage.


## Available Tools (4)
- **get_first_mention_distance**: Find distance to first symbol
- **verify_signature_placement**: Check for signature in tail
- **analyze_tag_distribution**: Analyze spacing between tags
- **count_entities**: Count @ mentions and # hashtags in a post


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Mention and Tag Distribution Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this LinkedIn post for tag distribution: 'Excited to be joining the team! #newjob #hiring @acme_corp'"

**🤖 AI Agent:**
> The post contains 2 hashtags and 1 mention. The first symbol appears at index 45.

---

**👤 You:**
> "Check if my LinkedIn post has a good signature block: 'Great day at the office! #worklife @team'"

**🤖 AI Agent:**
> The signature block check shows symbols are present in the final 50 characters.

---

**👤 You:**
> "How many mentions and hashtags are in this text? 'Hello world #news @vinkius'"

**🤖 AI Agent:**
> There is 1 mention and 1 hashtag found in the content.


## ❓ FAQ

**Q: What does this tool analyze?**
It identifies the distribution and density of @mentions and #hashtags within your LinkedIn post text.

**Q: How is clustering measured?**
The `analyze_tag_distribution` tool calculates the standard deviation of gaps between symbols to determine if they are clumped or evenly spaced.

**Q: Can it detect signature blocks?**
Yes, use `verify_signature_placement` to see if mentions appear in the final 50 characters of your post.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-mention-and-tag-distribution-checker](https://vinkius.com/mcp/linkedin-mention-and-tag-distribution-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Mention and Tag Distribution Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-mention-and-tag-distribution-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Mention and Tag Distribution Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-mention-and-tag-distribution-checker": {
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

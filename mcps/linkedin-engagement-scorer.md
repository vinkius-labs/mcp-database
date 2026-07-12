# LinkedIn Engagement Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-engagement-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Quantify the effectiveness of LinkedIn post Call-to-Actions (CT0As) and engagement triggers in text.

## Description
This MCP server provides a deterministic engine to evaluate LinkedIn posts for engagement potential. Using tools like `evaluate_linkedin_engagement` and `evaluate_scroll_stopper`, users can analyze text content for CTA markers, punctuation diversity, and sentence rhythm to determine stopping power and engagement probability. It acts as a bridge between your LinkedIn strategy and AI-driven analysis via Vinkius Edge.


## Available Tools (2)
- **evaluate_linkedin_engagement**: Evaluate the engagement potential of a LinkedIn post
- **evaluate_scroll_stopper**: Evaluate if a text acts as a "scroll stopper"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Engagement Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this LinkedIn post: "Are you tired of low engagement? Click here to learn more! #marketing""

**🤖 AI Agent:**
> The post contains a clear CTA ("Click here") and has an engagement score of 75/100.

---

**👤 You:**
> "Is this text a good scroll stopper? "Stop scrolling! This is the secret to LinkedIn growth...""

**🤖 AI Agent:**
> Yes, the punctuation diversity and rhythm in this snippet provide high stopping power.

---

**👤 You:**
> "Evaluate the engagement potential of: "Check out my new blog post on SEO strategies.""

**🤖 AI Agent:**
> The engagement score is 45/100 due to a weak CTA marker.


## ❓ FAQ

**Q: How does the engagement scoring work?**
The `evaluate_linkedin_engagement` tool analyzes your text for specific Call-to-Action (CTA) markers and evaluates punctuation diversity to predict how well a post will drive interaction.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this MCP server to Claude Desktop, Cursor, VS Code, or Windsurf using your personal Connection Token from the Vinkius dashboard via V1nkius Edge.

**Q: Does it require an API key for LinkedIn?**
No, this tool analyzes the text content you provide directly; no LinkedIn API credentials are required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-engagement-scorer](https://vinkius.com/mcp/linkedin-engagement-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Engagement Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-engagement-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Engagement Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-engagement-scorer": {
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

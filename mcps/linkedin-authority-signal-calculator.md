# LinkedIn Authority Signal Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-authority-signal-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Quantify thought-leadership and authority markers in LinkedIn posts.

## Description
This MCP server provides a suite of linguistic analysis tools to measure professional influence on LinkedIn. Use `get_customer_centricity_ratio` to see if your content focuses on the reader, `get_data_point_density` to quantify evidence-based claims, `get_definitive_statement_count` to identify conviction through absolute language, and `get_self_promotion_ratio` to monitor brand mentions. It transforms qualitative text into quantitative authority metrics.


## Available Tools (4)
- **get_customer_centricity_ratio**: Returns a ratio.

Determine if the content focuses on the reader or the author
- **get_data_point_density**: Quantify the evidence-based nature of the text
- **get_definitive_statement_count**: Measure the level of conviction and certainty in the writing
- **get_self_promotion_ratio**: Identify if the post is primarily promotional or educational


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Authority Signal Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this LinkedIn post for authority: 'I am excited to announce that our team at TechCorp achieved 20% growth this year. We always strive for excellence.'"

**🤖 AI Agent:**
> Customer-centricity ratio: 0.0. Data point density: 15.0 per 100 words. Definitive statement count: 1.

---

**👤 You:**
> "How much self-promotion is in this text? 'Check out my new book on LinkedIn marketing. It's available now at mystore.com.'"

**🤖 AI Agent:**
> Self-promotion ratio: 0.12 (based on 'my' and 'mystore.com' relative to word count).

---

**👤 You:**
> "Evaluate the conviction in this statement: 'You must always follow the rules of engagement.'"

**🤖 AI Agent:**
> Definitive statement count: 2 ('must', 'always').


## ❓ FAQ

**Q: How does the customer-centricity ratio work?**
The tool compares the frequency of audience-focused pronouns like 'you' and 'your' against author-focused pronouns such as 'I', 'we', or 'my'.

**Q: What counts as a data point?**
The calculator identifies percentages (%), currency symbols ($ or €), and explicit numerical digits to determine the density of evidence in your text.

**Q: Can I analyze posts from other platforms?**
While optimized for LinkedIn, the linguistic markers analyzed are applicable to any professional text-based content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-authority-signal-calculator](https://vinkius.com/mcp/linkedin-authority-signal-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Authority Signal Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-authority-signal-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Authority Signal Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-authority-signal-calculator": {
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

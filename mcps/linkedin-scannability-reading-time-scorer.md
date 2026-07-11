# LinkedIn Scannability & Reading Time Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-scannability-reading-time-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Calculate exact scannability metrics for LinkedIn feeds, including reading time and mobile viewport impact.

## Description
This MCP server provides precise analytical metrics to optimize LinkedIn content for mobile users. By using tools like `get_reading_time`, you can estimate how long a reader will spend on your post based on a 200 WPM baseline. The `estimate_mobile_viewport_impact` tool predicts what percentage of your text is visible before the 'see more' prompt appears. Additionally, you can evaluate structural rhythm using `analyze_structural_rhythm` to identify walls of text, and ensure keyword placement via `check_f_pattern_compliance` to maximize engagement in high-speed scrolling environments.


## Available Tools (4)
- **analyze_structural_rhythm**: Analyzes the structural rhythm and scannability of a post
- **check_f_pattern_compliance**: Checks how well a post follows the F-pattern reading behavior
- **estimate_mobile_viewport_impact**: Estimates how much of a post is visible on mobile without scrolling
- **get_reading_time**: Calculates estimated reading time for a LinkedIn post


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Scannability & Reading Time Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated reading time for this LinkedIn post: 'LinkedIn is a great place for professionals to connect and share insights about the future of AI technology.'"

**🤖 AI Agent:**
> The estimated reading time for this post is 0.07 minutes.

---

**👤 You:**
> "Analyze the structural rhythm of this text: 'Success requires discipline. Hard work pays off. Consistency is key.'"

**🤖 AI Agent:**
> The post has a short sentence ratio of 1.0, indicating a very high structural rhythm suitable for quick scanning.

---

**👤 You:**
> "Check if the keyword 'strategy' is in the start zone of this paragraph: 'Our new strategy focuses on growth and scalability.'"

**🤖 AI Agent:**
> The keyword 'strategy' was found within the first three words of the paragraph, resulting in a compliance score of 1.0.


## ❓ FAQ

**Q: How is reading time calculated?**
The `get_reading_time` tool calculates the total word count and divides it by a standard professional reading speed of 200 words per minute.

**Q: Can I check if my keywords are placed correctly?**
Yes, use the `check_f_pattern_compliance` tool. It checks if your target keywords appear within the first three words of each paragraph to capture attention.

**Q: Does this help with mobile optimization?**
Absolutely. The `estimate_mobile_viewport_impact` tool helps you understand how much of your post is visible on a phone screen without the user needing to scroll.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-scannability-reading-time-scorer](https://vinkius.com/mcp/linkedin-scannability-reading-time-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Scannability & Reading Time Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-scannability-reading-time-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Scannability & Reading Time Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-scannability-reading-time-scorer": {
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

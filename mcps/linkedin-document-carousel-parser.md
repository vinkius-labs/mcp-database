# LinkedIn Document Carousel Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-document-carousel-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Analyze LinkedIn PDF carousels for readability, visual rhythm, and engagement.

## Description
This MCP server provides a specialized toolkit for auditing LinkedIn document carousels. It allows AI agents to parse raw text into individual slides using `extract_slides`, identify overcrowded pages with `analyze_density`, assess content consistency via `evaluate_rhythm`, and quantify engagement potential through `detect_hooks`. Perfect for creators ensuring their PDF carousels are optimized for mobile consumption and high swipe-through rates.


## Available Tools (4)
- **analyze_density**: Identifies slides that exceed word or character limits
- **detect_hooks**: Quantifies engagement-driving language at the end of slides
- **evaluate_rhythm**: Assesses the consistency of content length across slides
- **extract_slides**: Returns an array of slides.

Extracts individual slides from a raw text stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Document Carousel Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this text and tell me if any slides are too long: '[Slide 1] Welcome to the guide! --- [Slide 2] This slide is way too long because it contains a massive amount of text that definitely exceeds the three hundred character limit for optimal mobile reading.'"

**🤖 AI Agent:**
> Slide 2 is flagged as congested because it exceeds the 300-character threshold.

---

**👤 You:**
> "Check the engagement of these slides: '[Slide 1] Here is a secret... [Slide 2] ...that you won't believe!'"

**🤖 AI Agent:**
> The engagement score is high due to the detection of cliffhanger words like 'secret' and 'won't believe'.

---

**👤 You:**
> "Analyze the rhythm of this carousel: '[Slide 1] Short. [Slide 2] Medium length slide here. [Slide 3] Very long and detailed content that might disrupt the visual flow.'"

**🤖 AI Agent:**
> The rhythm is unstable due to high variance in word counts across the slides.


## ❓ FAQ

**Q: How do I use the `extract_slides` tool?**
Provide your carousel text as a single string. The tool looks for markers like [Slide 1] or --- to identify where each slide begins.

**Q: What defines a 'congested' slide?**
A slide is considered congested if it exceeds the character limit (300 characters) but stays within the word count limit.

**Q: Can this tool help improve my LinkedIn engagement?**
Yes. By using `detect_hooks`, you can identify if your slides end with compelling cliffhangers that encourage users to swipe through the entire deck.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-document-carousel-parser](https://vinkius.com/mcp/linkedin-document-carousel-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Document Carousel Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-document-carousel-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Document Carousel Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-document-carousel-parser": {
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

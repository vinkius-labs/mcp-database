# Meta Ad Creative Copy-Pairing Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meta-ad-creative-copy-pairing-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Score the alignment between Meta ad copy and visual descriptions to optimize performance.

## Description
Optimize your advertising performance by ensuring perfect synergy between text and imagery. This MCP server provides specialized tools to analyze Meta ad creatives across four critical dimensions: `calculate_keyword_overlap` for semantic alignment, `estimate_text_density` for visual clarity, `score_headline_redundancy` to prevent repetitive messaging, and `verify_cta_consistency` to ensure your Call to Action matches your brand promise. Use these tools to reduce bounce rates and improve engagement by maintaining high-quality, cohesive ad assets.


## Available Tools (4)
- **verify_cta_consistency**: Verify consistency between CTA and ad promise
- **score_headline_redundancy**: Score redundancy of a headline relative to primary text
- **calculate_keyword_overlap**: Calculate overlap between ad text and image description
- **estimate_text_density**: Estimate text density on a creative


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meta Ad Creative Copy-Pairing Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How well does my ad copy match this image description: 'Get 50% off all summer dresses today!' and 'A bright photo of flowing floral dresses in a sunny garden'?"

**🤖 AI Agent:**
> The overlap score is high. Shared keywords found: dresses, summer.

---

**👤 You:**
> "Is the text density too high for this ad? Text: 'Huge Summer Sale! Up to 70% off all items in store now!' and Visual Space: 15%"

**🤖 AI Agent:**
> The density rating is excessive. There is a high risk of clutter obscuring key visual elements.

---

**👤 You:**
> "Check if this headline is redundant: Headline: 'Summer Sale' and Primary Text: 'Our massive summer sale is finally here!'"

**🤖 AI Agent:**
> A high redundancy level was detected. The headline repeats information already present in the primary text.


## ❓ FAQ

**Q: How does the keyword overlap tool work?**
The `calculate_keyword_overlap` tool identifies significant shared words between your ad text and the image description to measure semantic reinforcement.

**Q: Can I check if my CTA is misleading?**
Yes, use `verify_cta_consistency` to ensure your button label (like 'Shop Now') aligns with the promise made in your ad copy.

**Q: Does this help with text-in-image guidelines?**
Absolutely. The `estimate_text_density` tool evaluates if the amount of text on your creative exceeds recommended visual clarity thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meta-ad-creative-copy-pairing-scorer](https://vinkius.com/mcp/meta-ad-creative-copy-pairing-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meta Ad Creative Copy-Pairing Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meta-ad-creative-copy-pairing-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meta Ad Creative Copy-Pairing Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meta-ad-creative-copy-pairing-scorer": {
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

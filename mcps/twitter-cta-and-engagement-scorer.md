# Twitter CTA and Engagement Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twitter-cta-and-engagement-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze Twitter/X posts for engagement effectiveness, classifying CTAs and detecting algorithmic triggers.

## Description
The Twitter CTA and Engagement Scorer provides a deterministic scoring engine to analyze X (formerly Twitter) posts for engagement effectiveness. It evaluates call-to-action types, detects algorithmic triggers, measures insight density for quote tweets, and calculates structural positioning weight. Use `cta_type_tool` to classify interaction intent, `engagement_triggers_tool` to find high-performance phrases, `quote_potential_tool` to estimate quote tweet incentive via verb density, and `positional_weight_tool` to determine CTA effectiveness based on its distance from the end of the post.


## Available Tools (4)
- **cta_type_tool**: Classify the type of Call to Action (CTA) in a tweet
- **engagement_triggers_tool**: Detect high-performance engagement triggers in a tweet
- **positional_weight_tool**: Calculate the effectiveness of CTA placement
- **quote_potential_tool**: Evaluate the potential for a tweet to be quoted/reposted


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twitter CTA and Engagement Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this tweet for engagement: 'RT if you agree! This is the best way to learn about MCP.'"

**🤖 AI Agent:**
> The tweet contains an exact match for a retweet trigger. CTA Type: Retweet Bait. Confidence Score: 0.95.

---

**👤 You:**
> "What is the engagement potential of this text: 'I think we should explore new technologies in AI development.'"

**🤖 AI Agent:**
> The insight score is 0.75 based on identified verb density.

---

**👤 You:**
> "Check the CTA position for: 'Check out this link: https://vinkius.com/blog/mcp' where the CTA starts at index 15."

**🤖 AI Agent:**
> The calculated weight is 0.42, as the CTA is located significantly far from the end of the tweet.


## ❓ FAQ

**Q: How does the tool identify engagement triggers?**
The `engagement_triggers_tool` performs exact string matching against known high-performance phrases like 'RT if you agree' or 'Reply with'.

**Q: Can I use this for threads?**
Yes, you can analyze individual tweets within a thread using the `cta_type_tool` and `positional_weight_tool` to evaluate their effectiveness.

**Q: What is insight density?**
It is measured by the `quote_potential_tool`, which calculates a score based on the frequency of action-oriented or cognitive verbs in your text.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twitter-cta-and-engagement-scorer](https://vinkius.com/mcp/twitter-cta-and-engagement-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twitter CTA and Engagement Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twitter-cta-and-engagement-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twitter CTA and Engagement Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twitter-cta-and-engagement-scorer": {
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

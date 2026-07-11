# Review Response Template Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/review-response-template-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Automated evaluation of business response quality, personalization, and tone alignment.

## Description
This MCP server provides a suite of tools to measure the effectiveness of business responses to customer reviews. It evaluates key dimensions such as personalization using `score_personalization`, checks for tone alignment with `evaluate_tone_alignment`, ensures negative feedback is addressed via `verify_resolution_adequacy`, calculates response efficiency with `calculate_length_efficiency`, and detects repetitive templates through `assess_template_uniqueness`.


## Available Tools (5)
- **calculate_length_efficiency**: Calculate length efficiency ratio
- **score_personalization**: Score how personalized a response is
- **verify_resolution_adequacy**: Verify if negative reviews have a resolution
- **evaluate_tone_alignment**: Check if response tone matches review sentiment
- **assess_template_uniqueness**: Assess template uniqueness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Review Response Template Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How personalized is this response: 'Hi John, thanks for the great feedback on our pizza!' to the review 'John: The pizza was amazing!'?"

**🤖 AI Agent:**
> The response is highly personalized because it correctly identifies the reviewer, John, and references the specific product mentioned.

---

**👤 You:**
> "Check if this response to a negative review is adequate: 'We are sorry for the bad experience. We will look into it.'"

**🤖 AI Agent:**
> The response contains an acknowledgment of the issue, but lacks a specific action offer or contact pathway to ensure resolution.

---

**👤 You:**
> "Is this response too long compared to the review: 'Review: Great! Response: We are so incredibly happy that you had such a wonderful time at our establishment and we look forward to seeing you again very soon!'?"

**🤖 AI Agent:**
> The length ratio is significantly high, suggesting the response is disproportionately long compared to the brief review.


## ❓ FAQ

**Q: How does the personalization score work?**
The `score_personalization` tool checks if the response includes specific details from the review, such as the reviewer's name or mentioned products.

**Q: Can it detect repetitive responses?**
Yes, the `assess_template_uniqueness` tool compares your current response against a provided history of previous responses to identify high similarity scores.

**Q: Does it handle negative reviews?**
Absolutely. The `verify_resolution_adequacy` tool specifically checks if negative reviews are met with appropriate acknowledgment and an offer of action.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/review-response-template-scorer](https://vinkius.com/mcp/review-response-template-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Review Response Template Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `review-response-template-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Review Response Template Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "review-response-template-scorer": {
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

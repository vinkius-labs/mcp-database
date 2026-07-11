# Ad Copy Compliance Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ad-copy-compliance-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Audit ad copy against platform character limits and content policies.

## Description
The Ad Copy Compliance Checker is a specialized validation engine designed to prevent ad rejection by auditing text against platform-specific constraints. It checks Google RSA headlines and descriptions, Meta Ads primary text, and X (Twitter) posts for character/pixel count violations. Beyond length limits, the tool performs deep linguistic audits using `analyze_ad_compliance` to detect prohibited absolute claims like 'guaranteed' or 'best', identifies excessive capitalization and punctuation, and verifies the presence of required regulatory disclosures. Use `calculate_compliance_score` to quantify the risk level based on detected violations.


## Available Tools (2)
- **analyze_ad_compliance**: Returns compliance status and found violations.

Analyze ad copy for prohibited claims
- **calculate_compliance_score**: Calculate a compliance score based on violations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ad Copy Compliance Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this Google Ad headline for compliance: 'The best way to lose weight guaranteed!'"

**🤖 AI Agent:**
> Violation detected: The headline contains prohibited absolute claims ('best', 'guandom'). Compliance score is significantly reduced.

---

**👤 You:**
> "Analyze this Meta Ad primary text: 'Get instant results now!!!'"

**🤖 AI Agent:**
> Violation detected: Excessive punctuation ('!!!') and prohibited claim ('instant') found in the text.

---

**👤 You:**
> "Calculate a compliance score for an ad with 3 violations."

**🤖 AI Agent:**
> The calculated compliance score is 40.


## ❓ FAQ

**Q: What platforms does this tool support?**
The tool specifically validates text for Google Ads (RSA), Meta Ads (Facebook/Instagram), and X (formerly Twitter) to ensure they meet platform-specific character limits.

**Q: How does the compliance score work?**
You can use `calculate_compliance_score` to determine a risk level. The engine calculates a score from 0-100, where each detected violation reduces the total score by 20 points.

**Q: Can it detect prohibited words?**
Yes, by using `analyze_ad_compliance`, the tool scans your text for absolute claims and prohibited keywords such as 'guaranteed', 'promise', or 'cure' that might trigger policy reviews.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ad-copy-compliance-checker](https://vinkius.com/mcp/ad-copy-compliance-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ad Copy Compliance Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ad-copy-compliance-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ad Copy Compliance Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ad-copy-compliance-checker": {
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

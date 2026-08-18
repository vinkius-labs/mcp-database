# AWS WAF Rules & Rate Limiting Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-waf-rules-rate-limiting-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Calculate AWS WAF capacity, rate limits, and rule complexity against best practices.

## Description
This MCP server provides deterministic calculations for AWS WAF (Web Application Firewall) configurations. It helps architects and security engineers validate their rule sets against AWS recommended limits and mandatory constraints. Use `calculate_waf_capacity` to determine total rule counts across Web ACLs and rule groups, `analyze_rate_limiting` to verify rate-based rule thresholds, and `evaluate_rule_complexity` to ensure nesting depth and condition counts stay within safe operational bounds.


## Available Tools (3)
- **analyze_rate_limiting**: Evaluates rate-based rule configurations against AWS minimum requirements and constraints
- **calculate_waf_capacity**: Calculates the total rule and resource capacity based on the number of Web ACLs and rule groups provided
- **evaluate_rule_complexity**: Checks if the logical structure of rules adheres to nesting and condition limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS WAF Rules & Rate Limiting Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate capacity for 5 Web ACLs with 50 rules each, and 10 rule groups with 20 rules each."

**🤖 AI Agent:**
> Total Web ACLs: 5. Total rules in ACLs: 250. Total rule groups: 10. Total rules in groups: 200.

---

**👤 You:**
> "Is a rate threshold of 50 requests per 5 minutes valid?"

**🤖 AI Agent:**
> No, the threshold is invalid because it is below the minimum requirement of 100 requests.

---

**👤 You:**
> "Check complexity for a rule with 6 levels of nesting and 12 conditions."

**🤖 AI Agent:**
> The configuration is invalid. It violates the nesting limit (max 5) and exceeds the recommended condition limit (max 10).


## ❓ FAQ

**Q: How do I check if my WAF rule count is too high?**
You can use the `calculate_waf_capacity` tool. It will return a list of capacity warnings if your planned number of rules or Web ACLs exceeds the recommended limits.

**Q: What is the minimum threshold for rate-based rules?**
The minimum allowed threshold for rate-based rules in AWS WAF is 100 requests per 5-minute window. The `analyze_rate_limiting` tool will flag any value below this.

**Q: Can I use this to check rule nesting depth?**
Yes, the `evaluate_rule_complexity` tool specifically checks if your nesting depth exceeds the recommended limit of 5 levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-waf-rules-rate-limiting-calculator](https://vinkius.com/ai-agent-connect/aws-waf-rules-rate-limiting-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS WAF Rules & Rate Limiting Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-waf-rules-rate-limiting-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS WAF Rules & Rate Limiting Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-waf-rules-rate-limiting-calculator": {
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

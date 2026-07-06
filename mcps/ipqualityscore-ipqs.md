# IPQualityScore (IPQS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipqualityscore-ipqs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Detect fraud, proxies, and malicious activity via IPQS API.

## Description
Empower your AI agents to protect your platform with IPQualityScore (IPQS). This MCP server allows you to perform real-time lookups for IPs, emails, URLs, and phone numbers to detect fraud, bots, and high-risk activity. Ideal for automating security checks and enhancing risk management.


## Available Tools (10)
- **ip_lookup**: Returns fraud scores, proxy/VPN detection results, and geographical data. Essential for identifying malicious users or automated bots during sign-up or transaction processes.

Analyzes an IP address for fraud and proxy detection
- **list_conversions**: Useful for e-commerce and affiliate management auditing.

Lists tracked conversions
- **list_fraud**: Essential for high-level security auditing and threat monitoring.

Lists recent fraud event logs
- **list_reports**: Useful for auditing recent security triggers.

Lists recent fraud reports
- **list_stats**: Useful for monitoring integration health.

Lists usage statistics for your account
- **phone_lookup**: Returns line type and risk indicators. Use for identity verification and fraud prevention.

Analyzes a phone number for fraud and risk
- **url_lookup**: Returns a risk score and classification of the site. Use this to audit suspicious links provided by users or found in communication.

Analyzes a URL for malicious activity
- **email_lookup**: Returns a risk score and validation flags. Use this to vet new user registrations and prevent fraudulent accounts.

Analyzes an email address for fraud and deliverability
- **get_account**: Use to verify plan status and current configuration.

Retrieves details about your IPQS account
- **get_credits**: Essential for ensuring the service remains active and within quota.

Retrieves credit usage and balance information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPQualityScore (IPQS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the IP address 8.8.8.8 for fraud risk."

**🤖 AI Agent:**
> I'll perform an IP lookup using IPQS to check for any malicious indicators.

---

**👤 You:**
> "Verify if the email address 'fraudster@test.com' is risky."

**🤖 AI Agent:**
> I'll use IPQS email validation to check the risk score for that address.

---

**👤 You:**
> "Check this URL for potential malware: http://malicious-site.com"

**🤖 AI Agent:**
> I'll perform a malicious URL lookup with IPQS for you.


## ❓ FAQ

**Q: How do I get IPQS API credentials?**
Log in to your IPQS account and navigate to Account Settings to find your Private API Key.

**Q: Which lookups are supported?**
This MCP supports real-time lookups for IP addresses, email addresses, URLs, and phone numbers.

**Q: Can I see my credit balance?**
Yes, the get_credits tool provides details about your remaining credits and usage statistics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipqualityscore-ipqs](https://vinkius.com/mcp/ipqualityscore-ipqs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IPQualityScore (IPQS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ipqualityscore-ipqs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IPQualityScore (IPQS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ipqualityscore-ipqs": {
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

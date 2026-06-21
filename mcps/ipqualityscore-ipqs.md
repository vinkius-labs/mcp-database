# IPQualityScore (IPQS) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipqualityscore-ipqs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ipqualityscore-ipqs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ipqualityscore-ipqs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Detect fraud, proxies, and malicious activity via IPQS API.

## Description
Empower your AI agents to protect your platform with IPQualityScore (IPQS). This MCP server allows you to perform real-time lookups for IPs, emails, URLs, and phone numbers to detect fraud, bots, and high-risk activity. Ideal for automating security checks and enhancing risk management.


## Available Tools
- **email_lookup**: Returns a risk score and validation flags. Use this to vet new user registrations and prevent fraudulent accounts.

Analyzes an email address for fraud and deliverability
- **get_account**: Use to verify plan status and current configuration.

Retrieves details about your IPQS account
- **get_credits**: Essential for ensuring the service remains active and within quota.

Retrieves credit usage and balance information
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


## Installation & Usage

To install and use the **IPQualityScore (IPQS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipqualityscore-ipqs](https://vinkius.com/mcp/ipqualityscore-ipqs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

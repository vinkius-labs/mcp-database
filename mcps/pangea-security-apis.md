# Pangea (Security APIs) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pangea-security-apis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Secure your AI applications with Pangea's comprehensive security APIs — scan for PII, redact sensitive data, audit logs, and check for embargoed IPs.

## Description
Integrate **Pangea** into your AI workflows to provide a robust security layer for LLM interactions and organizational data. This server provides a unified interface to Pangea's cloud-native security services.

### Key Capabilities

- **AI Security & Guarding** — Use `ai_guard_text` and `ai_guard_prompt` to detect prompt injections, PII, and malicious content before they reach your model or user.
- **Data Privacy** — Automatically redact sensitive information from plain text or structured JSON objects using `redact_text` and `redact_structured`.
- **Secure Auditing** — Maintain a tamper-proof record of activities with `audit_log` and perform natural language searches through your security history via `audit_search`.
- **Threat Intelligence** — Check for embargoed locations with `embargo_ip_check` and scan files for threats with `sanitize_file`.
- **Identity & Access** — Manage authentication flows, user sessions, and authorization tuples directly from your agent.

### How it works

1. Subscribe to this server
2. Enter your Pangea Token and Domain from the Pangea Console
3. Start securing your AI agents in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — Automate audit log analysis and threat intelligence checks within your existing tools.
- **AI Developers** — Implement safety rails and PII redaction for LLM inputs and outputs without building custom middleware.
- **Compliance Officers** — Quickly search and verify audit trails using natural language queries.


## Available Tools (40)
- **ai_guard_text**: Scan text for PII, malicious content, and prompt injections
- **aidr_chat_completions**: Guard LLM chat completions with integrated logging and tracing
- **audit_log_bulk**: Create multiple secure audit log entries
- **audit_log**: Create a single secure audit log entry
- **audit_search_results**: Paginate through audit search results
- **audit_search**: Search the audit log using natural language queries
- **authn_flow_complete**: Finalize the flow and receive session tokens
- **authn_flow_start**: Start a sign-up or sign-in flow
- **authn_flow_update**: Update flow state (e.g., submit password, OTP)
- **authn_session_list**: List active user sessions
- **authn_session_logout**: Invalidate sessions
- **authn_user_create**: Programmatically create a user
- **authz_check**: Check if a subject has permission for an action on a resource
- **authz_list_resources**: List all resources a subject can access
- **authz_tuple_create**: Define relationships for AuthZ
- **domain_whois**: Get WHOIS details for a domain
- **embargo_ip_check**: Check if an IP originates from an embargoed country
- **embargo_iso_check**: Check a 2-character ISO country code against embargo lists
- **file_scan**: Scan a file for malware
- **intel_reputation**: Retrieve reputation scores for domains, URLs, or file hashes
- **ip_geolocate**: Retrieve location data for an IP
- **ip_proxy**: Detect if an IP is a proxy
- **ip_reputation**: Get reputation score and verdict for an IP
- **ip_vpn**: Detect if an IP is a VPN
- **password_breached**: Check if a password hash prefix appears in breach data
- **redact_structured**: Redact specific fields in a JSON object using JSONPath
- **redact_text**: Redact sensitive data from plain text
- **sanitize_file**: Apply sanitization rules to a file and receive a cleaned version
- **share_delete**: Delete files or folders
- **share_folder_create**: Create folders in Secure Share
- **share_get**: Download a file or retrieve metadata
- **share_list**: List objects in a bucket or folder with filtering
- **unredact**: Decrypt data previously redacted using FPE
- **user_breached**: Check if an email, phone, or username appears in known data breaches
- **vault_decrypt**: Perform cryptographic decryption
- **vault_encrypt**: Perform cryptographic encryption
- **vault_get**: Retrieve item details or secret values from Vault
- **vault_key_generate**: Generate symmetric or asymmetric keys in Vault
- **vault_secret_store**: Store a secret or token in Vault
- **ai_guard_prompt**: Analyze and redact content in LLM inputs/outputs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pangea (Security APIs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Redact any PII from this text: 'My email is john.doe@example.com and I live in New York'."

**🤖 AI Agent:**
> I've processed the text using `redact_text`. The redacted version is: 'My email is <EMAIL> and I live in <LOCATION>'.

---

**👤 You:**
> "Search the audit logs for any 'login' events from the last 24 hours."

**🤖 AI Agent:**
> I've queried the audit logs using `audit_search`. I found 3 login events. Would you like to see the details for each entry?

---

**👤 You:**
> "Check if the IP address 1.1.1.1 is from an embargoed country."

**🤖 AI Agent:**
> Running `embargo_ip_check` for 1.1.1.1... The check returned that this IP is not associated with any embargoed countries.


## ❓ FAQ

**Q: How can I protect my LLM from prompt injections or malicious content?**
You can use the `ai_guard_prompt` tool to analyze LLM messages. It scans for prompt injections, PII, and other security risks, providing a safety score and redaction suggestions before the data is processed.

**Q: Can I search through my security logs using natural language?**
Yes! The `audit_search` tool allows you to query your secure audit logs using natural language or structured queries, making it easy to find specific events without complex SQL.

**Q: How do I automatically redact PII from a block of text?**
Use the `redact_text` tool. Simply provide the text, and Pangea will identify and mask sensitive information like emails, phone numbers, and names based on your configured rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pangea-security-apis](https://vinkius.com/mcp/pangea-security-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pangea (Security APIs)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pangea-security-apis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pangea (Security APIs)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pangea-security-apis": {
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

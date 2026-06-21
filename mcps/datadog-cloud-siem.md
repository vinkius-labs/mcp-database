# Datadog Cloud SIEM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog-cloud-siem)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage cloud security via Datadog — search security signals, triage alerts, and audit detection rules directly from any AI agent.

## Description
Connect your **Datadog** security module to any AI agent and take full control of your Cloud SIEM and threat hunting workflows through natural conversation.

### What you can do

- **Security Signal Search** — Execute ingestion searches returning critical threats detected by Datadog SIEM, CSPM, and CWS matching MITRE ATT&CK vectors
- **Signal Triaging** — Update the state of active threat alerts, transitioning signals from open to archived with audited false-positive justifications
- **Detection Rule Management** — List and retrieve exact logic for security rules identifying AWS CloudTrail deviations or Kubernetes root escalations
- **Rule Orchestration** — Construct new Cloud SIEM Log Detection rules by pushing raw name/message fields and specific Lucene query bindings
- **Threat Hunting** — Directly query raw Datadog logs with a 10s lookbehind to capture highly localized context matching malicious source IPs
- **Security Filter Auditing** — Retrieve global exclusion policies mapping to SIEM log pipelines to verify which low-value vectors are blocked

### How it works

1. Subscribe to this server
2. Enter your Datadog API Key and APP Key
3. Start managing your cloud security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts & SOC** — search for security signals and triage active threats in real-time
- **Incident Responders** — hunt for threats using raw log context and malicous IP tracking
- **Security Engineers** — manage and deploy new detection rules using natural language
- **Compliance Officers** — audit security filters and detection rule configurations across environments


## Available Tools (10)
- **create_detection_rule**: Accepts raw name/message fields, specific Lucene query bindings filtering for malicious activity, and severity levels (info, low, medium, high, critical). Auto-activates upon creation.

Construct a new Cloud SIEM Log Detection Rule
- **security_system_ping**: Test API authentication validity against the Security Module
- **delete_detection_rule**: Irreversible action. Pre-packaged rules provided by Datadog typically cannot be outright deleted (only disabled), making this primarily for user-created custom JSON rules.

Permanently delete a Datadog Security Detection Rule
- **get_raw_log_context**: Use this immediately after verifying an attacker footprint.

Additional threat hunt tool extracting exact log bounds (100 msgs)
- **get_detection_rule**: g. > 5 occurrences in 5 mins), severity bindings, tagging matrices, and Notification routing hooks tying into PagerDuty or Slack.

Retrieve the exact logic/queries for a specific Detection Rule
- **list_security_filters**: These filters inherently block high-volume, low-value logging vectors from ever reaching the SIEM evaluation engine in order to preserve compute budgets.

List Security Filter configurations
- **list_detection_rules**: Verifies the existence of proactive detections identifying AWS CloudTrail deviations, GCP anomalous IAM usage, and Kubernetes root escalations.

List configured Datadog Security Detection Rules
- **search_raw_logs**: Essential for rapid Threat Hunting before detection rules alert. Useful for extracting contextual VPC Flow Logs or application stack traces related to an active breach.

Directly query raw Datadog Logs over the past 15/m for Threat Hunting
- **search_signals**: Use lucene-based queries like "status:critical OR @usr.id:admin" to filter high severity indicators mapping to MITRE ATT&CK vectors.

Search Cloud SIEM Security Signals (Alerts) over the last 24h
- **triage_signal**: Transition signals directly from "open" to "archived", or from "archived" back to "open". If archiving, an official reason (e.g. "false_positive" or "testing_or_maintenance") must be assigned.

Modify the state of a Datadog SIEM Security Signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datadog Cloud SIEM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all critical security signals from the last 24h"

**🤖 AI Agent:**
> I found 3 critical signals. Highlights include 'Brute Force Attempt' on 'api-server' and 'Unauthorized S3 Bucket Access' in 'production-env'. Would you like to triage any of these?

---

**👤 You:**
> "Search logs for IP '1.2.3.4' to hunt for threats"

**🤖 AI Agent:**
> Searching Datadog logs for '1.2.3.4'... I found 15 related events in the last 15 minutes. The IP is attempting to access '/admin/login' with multiple incorrect passwords. I can provide the full contextual logs.

---

**👤 You:**
> "Archive security signal 'sig_123' as a false positive"

**🤖 AI Agent:**
> Signal 'sig_123' has been archived! State updated to 'archived' with reason: 'false_positive'. This action is logged in your Datadog security timeline.


## ❓ FAQ

**Q: Can my agent help me triage security alerts in Datadog?**
Yes. Use the 'triage_signal' tool. You can update active threats from 'open' to 'archived', providing a required justification like 'false_positive'. The agent will push the status update directly to the Datadog SIEM platform.

**Q: How do I search for malicious activities matching specific IP addresses?**
Use the 'get_raw_log_context' tool. Provide the suspicious IP address, and the agent will perform a threat-hunting search with a 10s lookbehind to capture highly localized context matching that source, helping you verify attacker footprints.

**Q: Can I see all active security detection rules through the agent?**
Absolutely. The 'list_detection_rules' tool returns all custom and prepackaged Datadog Cloud SIEM rules. Your agent can then inspect specific rule schemas to verify evaluation windows, trigger cases, and notification hooks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog-cloud-siem](https://vinkius.com/mcp/datadog-cloud-siem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Datadog Cloud SIEM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datadog-cloud-siem` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Datadog Cloud SIEM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datadog-cloud-siem": {
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

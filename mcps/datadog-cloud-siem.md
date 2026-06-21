# Datadog Cloud SIEM MCP Server

Manage cloud security via Datadog — search security signals, triage alerts, and audit detection rules directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog-cloud-siem)

## Overview
**Category:** fort-knox
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Datadog Cloud SIEM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog-cloud-siem](https://vinkius.com/mcp/datadog-cloud-siem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

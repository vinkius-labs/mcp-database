# Lacework (Cloud Security & CNAPP) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lacework-cloud-security-cnapp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Secure your cloud via Lacework — search security alerts, monitor vulnerabilities, and audit cloud asset inventory.

## Description
Connect your **Lacework (FortiCNAPP)** account to any AI agent and take full control of your cloud security posture and threat hunting through natural conversation.

### What you can do

- **Alert Orchestration** — Search and retrieve deep behavioral telemetry for security alerts, identifying anomalous Kubernetes executions or AWS IAM brute-forcing attempts directly from your agent
- **Vulnerability Management** — List critical CVEs executing on cloud hosts and monitor static image vulnerabilities in your container registries (ECR, DockerHub)
- **Emergency Incident Response** — Instantly search your entire infrastructure for specific CVE exposure (e.g., Log4j) to identify vulnerable nodes during zero-day events
- **Asset Inventory Audit** — Query the real-time cloud control-plane to enumerate running instances, unrestricted S3 buckets, and active networking perimeters
- **Threat Hunting (LQL)** — Execute specialized Lacework Query Language (LQL) requests to analyze vast datasets for anomalous login patterns or API key abuse
- **Compliance Monitoring** — List and audit global cloud security policies to ensure your infrastructure remains within regulatory and organizational norms

### How it works

1. Subscribe to this server
2. Enter your Lacework Account, Key ID, and Secret
3. Start monitoring your cloud security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts** — hunt for threats and investigate polygraph alerts through natural conversation without manual dashboard filtering
- **DevOps & SREs** — monitor container and host vulnerabilities to ensure only secure images are promoted through the CI/CD pipeline
- **Compliance Officers** — audit security policies and unrestricted cloud assets to maintain a robust organizational security posture


## Available Tools
- **list_container_vulnerabilities**: Examines ECR/DockerHub registries or direct cluster deployments for images carrying critical inherited CVEs at the filesystem level before CI/CD promotion blocks.

List static image vulnerabilities detected in Container Registries
- **get_alert**: Extracts precisely what baseline behavior was deviated from, providing deep contextual metadata such as explicit AWS Accounts involved, offending Container Image SHAs, and correlated external IP anomalies.

Get exact behavioral payloads and telemetry for an Alert
- **list_host_vulnerabilities**: Identifies running processes strictly matched against Critical or High CVEs (e.g., Log4j, Polkit) directly active inside EC2 or GCE instances.

List known vulnerabilities executing natively on Cloud Hosts/VMs
- **search_cloud_inventory**: Used to dynamically enumerate running instances, active networking perimeters, or unrestricted S3 buckets discovered by cross-account role polling.

Query the real-time Lacework Cloud Control-Plane Asset Inventory
- **search_alerts**: Fetches events mapping to anomalous Kubernetes executions, AWS IAM brute-forcing attempts, and massive container network exfiltrations spanning the specified time filter.

Search Cloud Security alerts dynamically across Lacework
- **search_cve_exposure**: Directly filters the entire cloud infrastructure footprint determining exactly which specific nodes (Machines) are currently vulnerable to the designated CVE (e.g. "CVE-2026-0001").

Search all integrated Machines/Instances for a specific CVE
- **list_security_policies**: Confirms whether Lacework will alert directly if an engineer violates structural norms (e.g., exposing port 22 directly to 0.0.0.0/0).

List all global Cloud Security Policies enforced by Lacework
- **list_lql_queries**: These extract precise cloud telemetry fields mapping user-defined compliance checks directly against the underlying dataset.

List all Lacework Query Language (LQL) structures
- **list_resource_groups**: Helps define what constitutes "Production" vs "Staging" in Policy evaluation engines.

List logical Resource Groups managing Lacework architectures
- **execute_query**: Produces bespoke output matrices tracking API keys bypassing IAM logic, anomalous login patterns, or Kubernetes process spawn trees.

Execute an LQL Threat Hunting Query on-demand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lacework (Cloud Security & CNAPP)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all Critical alerts from the last 24 hours"

**🤖 AI Agent:**
> Searching alerts… I've identified 3 Critical alerts in your Lacework account: 1) Anomalous Kubernetes Process, 2) AWS Root Account Access from new IP, 3) Massive Data Exfiltration detected. Which one would you like to investigate first?

---

**👤 You:**
> "List all host vulnerabilities for our Production resource group"

**🤖 AI Agent:**
> Retrieving host vulnerabilities… Found 12 active CVEs across 4 instances in the Production group. Highlights: 2 Critical (Log4j related) and 5 High impact. I can provide the Machine IDs and remediation steps for the critical ones.

---

**👤 You:**
> "Are there any unrestricted S3 buckets currently visible in our inventory?"

**🤖 AI Agent:**
> Auditing cloud inventory… I've discovered 2 unrestricted S3 buckets (AWS:S3:Bucket): 'public-assets-prod' and 'temp-data-dump'. Both allow world-readable access. Would you like to see the associated security policies for these assets?


## ❓ FAQ

**Q: Can I search for specific CVE exposure across my whole cloud environment?**
Yes. Use the `search_cve_exposure` tool and provide the official CVE ID (e.g. CVE-2023-1234). Your agent will filter the entire cloud footprint to determine exactly which specific nodes or machines are currently vulnerable.

**Q: How do I investigate the behavioral telemetry of a specific security alert?**
The `get_alert` tool extracts precisely what baseline behavior was deviated from for a specific Alert ID. Your agent will return detailed contextual metadata, including offending container SHAs and correlated IP anomalies.

**Q: Can my agent run custom threat hunting queries using LQL?**
Absolutely. Use the `execute_query` tool to run specialized Lacework Query Language (LQL) blocks. This allows your agent to perform complex mathematical analysis on cloud telemetry to identify deep security patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lacework-cloud-security-cnapp](https://vinkius.com/mcp/lacework-cloud-security-cnapp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lacework (Cloud Security & CNAPP)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lacework-cloud-security-cnapp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lacework (Cloud Security & CNAPP)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lacework-cloud-security-cnapp": {
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

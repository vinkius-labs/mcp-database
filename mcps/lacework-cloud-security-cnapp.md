# Lacework (Cloud Security & CNAPP) MCP Server

Secure your cloud via Lacework — search security alerts, monitor vulnerabilities, and audit cloud asset inventory.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lacework-cloud-security-cnapp)

## Overview
**Category:** fort-knox
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Lacework (Cloud Security & CNAPP)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lacework-cloud-security-cnapp](https://vinkius.com/mcp/lacework-cloud-security-cnapp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

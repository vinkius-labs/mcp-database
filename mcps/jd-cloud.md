# JD Cloud / 京东云 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jd-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jd-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jd-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading supply chain cloud platform — manage VMs, storage, and cloud infrastructure via AI.

## Description
Empower your AI agent to orchestrate your cloud infrastructure and supply chain assets with **JD Cloud** (京东云), the premier cloud service provider by JD.com. By connecting JD Cloud to your agent, you transform complex virtual machine management, storage bucket auditing, and billing analysis into a natural conversation. Your agent can instantly retrieve VM instance details, list Object Storage Service (OSS) buckets, audit VPC networks, and retrieve comprehensive billing summaries without you ever needing to navigate the comprehensive JD Cloud Console. Whether you are managing e-commerce backend resources or coordinating high-volume digital distribution, your agent acts as a real-time cloud operations assistant, providing accurate results from a single, authorized source.

### What you can do

- **Compute Orchestration** — List virtual machines, retrieve detailed instance metadata, and monitor operational status.
- **Storage Auditing** — List Object Storage Service (OSS) buckets and manage cloud disk resources across regions.
- **Network Management** — Retrieve details for Virtual Private Clouds (VPC) and coordinate network topology audits.
- **Financial Auditing** — Retrieve comprehensive billing summaries for specific time ranges to maintain cost control.
- **Operational Monitoring** — Verify project connectivity, active regions, and retrieve IAM account profile details.

### How it works

1. Subscribe to this server
2. Enter your JD Cloud Access Key, Secret Key, and Region
3. Start managing your cloud infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SRE Engineers** — automate routine infrastructure audits and monitor system health through natural language.
- **IT Financial Managers** — audit cloud spending and retrieve billing summaries directly from your AI-powered workspace.
- **Developers** — integrate professional-grade JD Cloud APIs into your AI-driven daily routines.
- **JD Cloud Power Users** — integrate your existing cloud projects into your AI-driven daily routines.


## Available Tools
- **get_account_profile**: Get IAM user info
- **get_billing_summary**: Get billing overview
- **get_vm_detail**: Get VM metadata
- **list_cicd_pipelines**: List DevOps pipelines
- **list_cloud_disks**: List block storage disks
- **list_oss_buckets**: List storage buckets
- **list_vm_instances**: List virtual machines
- **list_vpc_networks**: List VPC networks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JD Cloud / 京东云** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my running virtual machines in region 'cn-north-1'."

**🤖 AI Agent:**
> I've retrieved your VM instances for the Beijing region. You have 3 active instances: 'Web_Server_01' (Running), 'DB_Master' (Running), and 'Test_Lab' (Stopped). Would you like to see the detailed specs for the 'Web_Server_01'?

---

**👤 You:**
> "Check our JD Cloud billing summary from October 1st to October 15th."

**🤖 AI Agent:**
> I've retrieved the billing summary for your account. For the requested period, the total expenditure was 1,240.50 CNY. The largest cost contributors were VM instances (65%) and OSS storage (20%). Should I check the detailed usage for VM resources?

---

**👤 You:**
> "Show me the list of Object Storage (OSS) buckets in my account."

**🤖 AI Agent:**
> I've retrieved your OSS bucket list. You have 5 buckets configured, including 'assets-prod', 'backup-logs', and 'user-uploads'. Would you like me to check the region and creation date for a specific bucket?


## Installation & Usage

To install and use the **JD Cloud / 京东云** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jd-cloud](https://vinkius.com/mcp/jd-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

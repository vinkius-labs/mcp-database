# JD Cloud Infrastructure MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jd-cloud-infrastructure)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage JD Cloud supply-chain infrastructure from your AI. Control VMs, disks, databases, and monitor resource metrics.

## Description
Connect your AI agents directly to **JD Cloud** (京东云), the enterprise cloud infrastructure backing one of the world's largest e-commerce and supply chain platforms. This MCP provides 11 power tools spanning the full infrastructure lifecycle.

### What you can do

- **VM Lifecycle Management** — List, inspect, start, stop, and reboot virtual machines through natural language
- **Storage Operations** — Enumerate and inspect cloud disks and Object Storage buckets
- **Network Oversight** — Query Elastic IP allocations and their association status
- **Database Administration** — List RDS instances with engine versions and connection status
- **Performance Monitoring** — Pull time-series CPU, network, and disk metrics for any resource

### How it works

1. Navigate to the [JD Cloud Console](https://console.jdcloud.com/) and generate IAM Access Keys
2. Insert your **Access Key**, **Secret Key**, and preferred **Region ID** into Vurb
3. The MCP engine constructs the `JDCLOUD2-HMAC-SHA256` signature locally for every request.

### Who is this for?

- **DevOps Engineers** — Manage cloud infrastructure via conversational AI without switching dashboards
- **SRE Teams** — Query real-time metrics and restart unhealthy instances through automated agents
- **Supply Chain Architects** — Oversee the cloud backbone powering JD's logistics network


## Available Tools
- **describe_cloud_disk**: Get detailed information about a specific cloud disk
- **describe_vm_instance**: Get detailed information about a specific VM instance
- **describe_metric_data**: Query monitoring metric data for a cloud resource
- **list_oss_buckets**: List all Object Storage Service buckets
- **list_cloud_disks**: List all cloud disk volumes in your region
- **list_elastic_ips**: List all Elastic IP addresses in your region
- **list_vm_instances**: List all virtual machine instances in your JD Cloud region
- **list_rds_instances**: List all RDS database instances in your region
- **reboot_vm_instance**: Reboot a VM instance
- **start_vm_instance**: Start a stopped VM instance
- **stop_vm_instance**: Stop a running VM instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JD Cloud Infrastructure** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my running virtual machines on JD Cloud."

**🤖 AI Agent:**
> I queried the VM service and found 4 instances: 2 running (i-abc123, i-def456), 1 stopped (i-ghi789), and 1 in maintenance (i-jkl012). Total allocated vCPUs: 16.

---

**👤 You:**
> "Show me the CPU usage for instance i-abc123 over the last hour."

**🤖 AI Agent:**
> I pulled cpu.util metrics for i-abc123. Average CPU usage: 34.2%, peak: 78.9% at 23:42 UTC. The instance appears healthy with no sustained high-load periods.


## ❓ FAQ

**Q: Is the JDCLOUD2-HMAC-SHA256 signing handled automatically?**
Yes. The MCP engine locally derives signing keys through HMAC chains (date → region → service → jdcloud2_request), constructs canonical requests, and injects the Authorization header transparently. Your AI never handles raw crypto.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jd-cloud-infrastructure](https://vinkius.com/mcp/jd-cloud-infrastructure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JD Cloud Infrastructure** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jd-cloud-infrastructure` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JD Cloud Infrastructure** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jd-cloud-infrastructure": {
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

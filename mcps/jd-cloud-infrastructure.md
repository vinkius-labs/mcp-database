# JD Cloud Infrastructure MCP Server

Manage JD Cloud supply-chain infrastructure from your AI. Control VMs, disks, databases, and monitor resource metrics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jd-cloud-infrastructure)

## Overview
**Category:** industry-titans
**Tools Count:** 11

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


## Installation & Usage

To install and use the **JD Cloud Infrastructure** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jd-cloud-infrastructure](https://vinkius.com/mcp/jd-cloud-infrastructure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

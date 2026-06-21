# CoreWeave (AI GPU Cloud) MCP Server

Manage high-performance AI infrastructure on CoreWeave — provision GPU clusters, configure VPCs, and orchestrate inference gateways directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coreweave-ai-gpu-cloud)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 24

## Description
Connect your **CoreWeave** account to any AI agent to manage specialized GPU cloud infrastructure through natural language conversation.

### What you can do

- **Kubernetes Clusters (CKS)** — List, create, and manage bare-metal Kubernetes clusters optimized for intensive AI and ML workloads.
- **Network Isolation (VPC)** — Configure Virtual Private Clouds to ensure secure, isolated networking for your compute resources.
- **Inference Gateways** — Orchestrate gateways for routing and authenticating traffic to your deployed AI models.
- **Deployment Monitoring** — List and inspect inference deployments to ensure your services are running at peak performance.
- **Resource Lifecycle** — Full CRUD operations for clusters, VPCs, and gateways to automate your infrastructure scaling.

### How it works

1. Subscribe to this server
2. Enter your CoreWeave API Token
3. Start managing your GPU cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **ML Engineers** — Provision and scale GPU clusters without leaving your development environment.
- **DevOps Teams** — Automate VPC setup and gateway routing for production-grade AI services.
- **AI Researchers** — Quickly inspect cluster status and deployment health during model training or testing phases.


## Available Tools
- **get_vpc**: Get details for a specific VPC
- **create_capacity_claim**: Create a new Inference Capacity Claim
- **create_cluster**: Create a new CKS cluster
- **update_cluster**: Requires an updateMask in the payload.

Update a CKS cluster
- **update_deployment**: Update an Inference Deployment
- **update_gateway**: Update an Inference Gateway
- **update_vpc**: Update a VPC
- **create_deployment**: Create a new Inference Deployment
- **create_gateway**: Create a new Inference Gateway
- **create_vpc**: Create a new VPC
- **delete_capacity_claim**: Delete an Inference Capacity Claim
- **delete_cluster**: Delete a CKS cluster
- **delete_deployment**: Delete an Inference Deployment
- **delete_gateway**: Delete an Inference Gateway
- **delete_vpc**: Delete a VPC
- **get_cluster**: Get details for a specific CKS cluster
- **list_capacity_claims**: List all Inference Capacity Claims
- **list_clusters**: List all CoreWeave Kubernetes Service (CKS) clusters
- **list_deployments**: List all Inference Deployments
- **list_gateways**: List all Inference Gateways
- **list_vpcs**: List all Virtual Private Clouds (VPCs)
- **query_logs**: Query Loki logs
- **query_metrics**: Query Prometheus metrics
- **update_capacity_claim**: Update an Inference Capacity Claim


## Installation & Usage

To install and use the **CoreWeave (AI GPU Cloud)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coreweave-ai-gpu-cloud](https://vinkius.com/mcp/coreweave-ai-gpu-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

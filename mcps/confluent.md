# Confluent MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/confluent)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/confluent-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/confluent-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enable your AI agent to manage Kafka clusters, topics, and environments via the Confluent Cloud API.

## Description
Connect your AI to **Confluent Cloud**, the fully managed data streaming platform built on Apache Kafka.

### What you can do

- **Cluster Monitoring** — Check the health and status of your Kafka clusters, including node availability and CPU metrics.
- **Topic Management** — List, create, and inspect topics, check partition health, and review recent event flows.
- **Environment Audits** — Query environments to list active connectors and verify configuration states.

### How it works

1. Add the Confluent integration to your AI toolset.
2. Provide your Cloud API Key and Secret.
3. Monitor and manage your streaming infrastructure via natural language.

### Who is this for?

- **Data Engineers** — Verify pipelines and create streaming topics on the fly.
- **DevOps Teams** — Monitor cluster health and review configurations without opening the dashboard.
- **System Architects** — Audit streams and schema registries while planning new integrations.


## Available Tools
- **get_cluster_details**: Returns configuration, endpoint URLs, availability, and provisioning status.

Retrieve detailed information about a specific Kafka cluster
- **list_cloud_api_keys**: Retrieve API keys in the Confluent Cloud account
- **list_clusters**: Returns all Kafka clusters with their status, cloud provider, and region.

Retrieve Kafka clusters in a specific environment
- **list_connectors**: Returns configured source and sink connectors with their status.

Retrieve Kafka Connect connectors in an environment and cluster
- **list_environments**: Use this to discover environment IDs needed for cluster and connector operations.

Retrieve a list of Confluent Cloud environments
- **list_service_accounts**: Useful for auditing programmatic access.

Retrieve service accounts in the Confluent Cloud organization
- **list_topics**: Returns all topics with partition count and replication configuration.

Retrieve topics in a specific Kafka cluster


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Confluent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the health of the 'main-eu' Kafka cluster."

**🤖 AI Agent:**
> Cluster 'main-eu' is healthy. All nodes are available, CPU utilization averages 42%, and no alerts have been logged in the past 24 hours.

---

**👤 You:**
> "List all active topics in the 'default_env' environment."

**🤖 AI Agent:**
> 8 topics found in 'default_env':
1. 'user-actions' — 12 partitions, 2.3K msgs/sec
2. 'payment-events' — 6 partitions, 850 msgs/sec
3. 'analytics-pipeline' — 8 partitions, 1.1K msgs/sec
Would you like partition details for any of these?

---

**👤 You:**
> "Check the status of the 'mysql-source' connector."

**🤖 AI Agent:**
> The 'mysql-source' connector is actively running. There are 0 failed tasks, and it has successfully processed 45,000 records in the last hour.


## Installation & Usage

To install and use the **Confluent** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/confluent](https://vinkius.com/mcp/confluent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

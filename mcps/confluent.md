# Confluent MCP Server

Enable your AI agent to manage Kafka clusters, topics, and environments via the Confluent Cloud API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/confluent)

## Overview
**Category:** industry-titans
**Tools Count:** 7

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


## Installation & Usage

To install and use the **Confluent** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/confluent](https://vinkius.com/mcp/confluent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
